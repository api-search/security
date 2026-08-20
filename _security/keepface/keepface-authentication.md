---
api_key_in:
- header
auth_types:
- hmac
- bearer
- origin-allowlist
- none
description: ''
kind: authentication
layout: security
method: searched
name: Keepface Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeepFace secures its APIs with hmac, bearer, origin-allowlist, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KeepFace
provider_slug: keepface
scheme_count: 5
schemes:
- algorithm: HMAC-SHA256
  applies_to:
  - POST /api/v2/affiliate/postback/{brand_id}
  - POST /api/v2/affiliate/postback/{brand_id}/refund
  construction: signature = lowercase(hex(HMAC-SHA256(brand_secret, signed_payload)))
  failure: 401 {"error":"invalid_signature"}
  headers:
    signature: X-KF-Signature
    timestamp: X-KF-Timestamp
  name: hmac-body-signature
  replay_protection:
    enabled: true
    format: unix epoch seconds
    header: X-KF-Timestamp
    on_violation: 401 {"error":"stale_timestamp"}
    remediation: sync the calling server clock to NTP
    tolerance_seconds: 300
  secret:
    env_var_convention: KF_AFFILIATE_SECRET
    location: Brands > Edit > Affiliate > Tracking tab > Generate secret
    name: brand secret
    note: after rotation the previous secret stays valid for 7 days so the caller can roll without downtime
    overlap_on_rotation_days: 7
    rotatable: true
    shown_once: true
  signature_encoding: lowercase hex
  signed_payload: <timestamp> + "." + <raw_body>
  surface: Affiliate API v2 — postback and refund
  type: hmac
- algorithm: HMAC-SHA256
  applies_to:
  - POST /api/v2/affiliate/shopify/{brand_id}
  construction: base64(hmac_sha256(shopify_secret, raw_body))
  failure: 412 {"error":"shopify_not_configured"} when the brand has no Shopify secret set
  headers:
    signature: X-Shopify-Hmac-Sha256
  name: shopify-webhook-hmac
  note: standard Shopify webhook verification; the shared secret is the Shopify app secret configured per brand
  signature_encoding: base64
  surface: Affiliate API v2 — Shopify receiver
  type: hmac
- applies_to:
  - OPTIONS /api/v2/affiliate/pixel/{brand_id}
  - POST /api/v2/affiliate/pixel/{brand_id}
  configuration: Brands > Edit > Affiliate > Tracking > Allowed pixel origins
  mechanism: browser Origin header checked against a per-brand allowlist
  name: pixel-origin-allowlist
  note: Deliberately not a shared secret — the pixel runs in the buyer's browser, so the origin allowlist plus server-side anti-fraud is the control. Brands that need stronger assurance are directed to the server-side postback instead.
  surface: Affiliate API v2 — browser JS pixel
  type: origin-allowlist
- applies_to:
  - GET /api/v2/affiliate/resolve/{token}
  mechanism: unauthenticated; the 8-character affiliate token in the path is itself the capability
  name: none-public-resolve
  surface: Affiliate API v2 — click resolve
  token_format: mixed-case base62, 8 characters, case-sensitive
  type: none
  verified: probed anonymously 2026-08-13; a well-formed unknown token returns 404 (cached 60s) and a malformed token returns 400 (cached 300s), both as JSON, with X-RateLimit-Limit 600 present on the response.
- default_expiry_days: 90
  discovery_metadata: none (no /.well-known/oauth-protected-resource, HTTP 404)
  expiry_configurable: true
  failure: 401 {"error":"missing bearer token"} — observed live on an anonymous tools/list POST, 2026-08-13
  format: Bearer kf_<token>
  header: Authorization
  in: header
  issued_by: Settings, API Tokens (per brand workspace)
  name: mcp-bearer-token
  note: Static long-lived credential, not an OAuth access token. There is no authorization endpoint, no refresh, and no dynamic client registration; a human must create the token in the panel and paste it into the agent's MCP configuration.
  oauth: false
  revocable: true
  scheme: bearer
  scoped: true
  scopes_file: ../scopes/keepface-scopes.yml
  shown_once: true
  surface: MCP server (https://mcp.keepface.com/mcp)
  token_prefix: kf_
  type: http
  workspace_pinned: true
slug: keepface-authentication
source_filename: keepface-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.keepface.com/brand/affiliate-program/api-reference/\ndocs:\n- https://help.keepface.com/brand/affiliate-program/api-reference/\n- https://help.keepface.com/brand/affiliate-program/postback-hmac-integration/\n- https://help.keepface.com/brand/integrations/manage-with-claude-code/\n\n# Derived from the provider's published documentation, not from an OpenAPI —\n# Keepface publishes no machine-readable spec. Every scheme below is quoted from\n# a help-centre page and, where noted, confirmed against a live response.\n\nsummary:\n  types: [hmac, bearer, origin-allowlist, none]\n  oauth2: false\n  openid_connect: false\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Keepface runs two distinct auth models on two distinct surfaces. The public\n    Affiliate API v2 is machine-to-machine and authenticates each request by\n    HMAC-SHA256 body signature with a per-brand shared secret; there is no\n    bearer token\
  \ and no OAuth. The MCP server authenticates with a static,\n    workspace-pinned bearer token created by a human in the panel. Neither\n    surface implements OAuth 2.0 or OIDC, and no /.well-known/ auth metadata is\n    served on any host.\n\nschemes:\n\n- name: hmac-body-signature\n  surface: Affiliate API v2 — postback and refund\n  type: hmac\n  algorithm: HMAC-SHA256\n  applies_to:\n  - POST /api/v2/affiliate/postback/{brand_id}\n  - POST /api/v2/affiliate/postback/{brand_id}/refund\n  headers:\n    signature: X-KF-Signature\n    timestamp: X-KF-Timestamp\n  signature_encoding: lowercase hex\n  signed_payload: '<timestamp> + \".\" + <raw_body>'\n  construction: 'signature = lowercase(hex(HMAC-SHA256(brand_secret, signed_payload)))'\n  replay_protection:\n    enabled: true\n    header: X-KF-Timestamp\n    format: unix epoch seconds\n    tolerance_seconds: 300\n    on_violation: '401 {\"error\":\"stale_timestamp\"}'\n    remediation: sync the calling server clock to NTP\n  secret:\n\
  \    name: brand secret\n    env_var_convention: KF_AFFILIATE_SECRET\n    location: Brands > Edit > Affiliate > Tracking tab > Generate secret\n    shown_once: true\n    rotatable: true\n    overlap_on_rotation_days: 7\n    note: after rotation the previous secret stays valid for 7 days so the caller can\n      roll without downtime\n  failure: '401 {\"error\":\"invalid_signature\"}'\n\n- name: shopify-webhook-hmac\n  surface: Affiliate API v2 — Shopify receiver\n  type: hmac\n  algorithm: HMAC-SHA256\n  applies_to:\n  - POST /api/v2/affiliate/shopify/{brand_id}\n  headers:\n    signature: X-Shopify-Hmac-Sha256\n  signature_encoding: base64\n  construction: 'base64(hmac_sha256(shopify_secret, raw_body))'\n  note: standard Shopify webhook verification; the shared secret is the Shopify app\n    secret configured per brand\n  failure: '412 {\"error\":\"shopify_not_configured\"} when the brand has no Shopify secret\n    set'\n\n- name: pixel-origin-allowlist\n  surface: Affiliate API v2 —\
  \ browser JS pixel\n  type: origin-allowlist\n  applies_to:\n  - OPTIONS /api/v2/affiliate/pixel/{brand_id}\n  - POST /api/v2/affiliate/pixel/{brand_id}\n  mechanism: browser Origin header checked against a per-brand allowlist\n  configuration: Brands > Edit > Affiliate > Tracking > Allowed pixel origins\n  note: >-\n    Deliberately not a shared secret — the pixel runs in the buyer's browser, so\n    the origin allowlist plus server-side anti-fraud is the control. Brands that\n    need stronger assurance are directed to the server-side postback instead.\n\n- name: none-public-resolve\n  surface: Affiliate API v2 — click resolve\n  type: none\n  applies_to:\n  - GET /api/v2/affiliate/resolve/{token}\n  mechanism: unauthenticated; the 8-character affiliate token in the path is itself\n    the capability\n  token_format: mixed-case base62, 8 characters, case-sensitive\n  verified: >-\n    probed anonymously 2026-08-13; a well-formed unknown token returns 404\n    (cached 60s) and a malformed\
  \ token returns 400 (cached 300s), both as JSON,\n    with X-RateLimit-Limit 600 present on the response.\n\n- name: mcp-bearer-token\n  surface: MCP server (https://mcp.keepface.com/mcp)\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer kf_<token>'\n  token_prefix: kf_\n  in: header\n  issued_by: Settings, API Tokens (per brand workspace)\n  shown_once: true\n  default_expiry_days: 90\n  expiry_configurable: true\n  revocable: true\n  scoped: true\n  scopes_file: ../scopes/keepface-scopes.yml\n  workspace_pinned: true\n  oauth: false\n  discovery_metadata: none (no /.well-known/oauth-protected-resource, HTTP 404)\n  failure: '401 {\"error\":\"missing bearer token\"} — observed live on an anonymous\n    tools/list POST, 2026-08-13'\n  note: >-\n    Static long-lived credential, not an OAuth access token. There is no\n    authorization endpoint, no refresh, and no dynamic client registration; a\n    human must create the token in the panel and paste it into the\
  \ agent's MCP\n    configuration.\n\nnot_supported:\n- oauth2\n- openid-connect\n- mutual-tls\n- basic-auth\n- api-key-query-parameter\n\nx-evidence:\n- {url: 'https://api.keepface.ai/api/v2/affiliate/resolve/zzzz', http_status: 400,\n  note: anonymous, JSON body, x-ratelimit-limit 600, fetched '2026-08-13'}\n- {url: 'https://mcp.keepface.com/mcp', http_status: 401, note: 'anonymous POST tools/list\n    returns {\"error\":\"missing bearer token\"}', fetched: '2026-08-13'}\n- {url: 'https://help.keepface.com/brand/affiliate-program/api-reference/', http_status: 200,\n  fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keepface/refs/heads/main/authentication/keepface-authentication.yml
summary_line: hmac/bearer/origin-allowlist/none · 5 schemes
tags:
- Company
- Influencer Marketing
- Creator Economy
- Marketing
- Social-Media
- Affiliate Marketing
- Advocacy
- Campaign Management
- MCP
- AI Agents
- Attribution
- Webhook
---
