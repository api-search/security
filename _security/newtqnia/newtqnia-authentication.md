---
api_key_in: []
api_specs:
- filename: newtqnia-news-api-openapi.yml
  format: yaml
  label: NewTqnia | Technology News, AI and Innovation News API
  slug: newtqnia-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newtqnia/refs/heads/main/openapi/newtqnia-news-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Newtqnia Authentication
name_suffix: Authentication
oauth_flows: []
overview: NewTqnia | Technology News, AI and Innovation declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: NewTqnia | Technology News, AI and Innovation
provider_slug: newtqnia
scheme_count: 0
schemes: []
slug: newtqnia-authentication
source_filename: newtqnia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://newtqnia.com/en/developers + https://newtqnia.com/en/connect + https://newtqnia.com/.well-known/oauth-authorization-server\ndocs: https://newtqnia.com/en/connect\nnote: >-\n  derive-authentication.py found ZERO securitySchemes because the published OpenAPI 3.1\n  contract declares none - it models the API key as an optional header PARAMETER\n  (components.parameters.ApiKey, X-API-Key, required:false) rather than as a\n  securityScheme. That is a real contract gap, recorded under gaps[] below; this profile\n  is written from the provider's own documentation and from the live OAuth metadata.\n\nsummary: >-\n  The REST Daily Digest API is genuinely keyless - the public endpoints answered 200\n  anonymously in our probe. An optional ntq_-prefixed API key plus two optional\n  attribution headers identify the caller for usage accounting. The MCP server is the\n  gated surface: it accepts the same personal API key over X-API-Key\
  \ or Authorization:\n  Bearer, and additionally supports OAuth 2.1 authorization_code + PKCE for clients that\n  cannot send a custom header.\n\nsurfaces:\n- surface: REST Daily Digest API\n  base_url: https://api.newtqnia.com\n  auth_required: false\n  verified: probed\n  evidence: 'GET https://api.newtqnia.com/v1/news/today?limit=1 -> 200 with no credential'\n  schemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    required: false\n    prefix: ntq_\n    purpose: >-\n      Optional traffic identifier. Public endpoints remain accessible without a key. A\n      website origin is treated as verified only when associated with a recognized key.\n  attribution_headers:\n  - name: X-NewTqnia-Application\n    in: header\n    required: false\n    max_length: 120\n    purpose: Caller application name for usage attribution.\n  - name: X-NewTqnia-Website\n    in: header\n    required: false\n    format: uri\n    purpose: Public website origin; verified only when tied to a recognized\
  \ key.\n\n- surface: MCP server\n  base_url: https://newtqnia.com/mcp\n  auth_required: true\n  auth_required_for: tool invocation only\n  verified: probed\n  evidence: >-\n    initialize and tools/list both returned 200 anonymously; the provider documents that\n    calling a tool requires a personal key or an OAuth token.\n  schemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    prefix: ntq_\n  - type: http\n    scheme: bearer\n    name: Authorization\n    format: 'Bearer ntq_...'\n    note: Same personal key, for clients offering only a bearer-token field.\n  - type: oauth2\n    flow: authorization_code\n    pkce_methods: [S256]\n    authorization_endpoint: https://newtqnia.com/oauth/authorize\n    token_endpoint: https://newtqnia.com/oauth/token\n    issuer: https://newtqnia.com\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    authorization_response_iss_parameter_supported: true\n   \
  \ scopes: [mcp:read, mcp:write]\n    discovery:\n    - https://newtqnia.com/.well-known/oauth-authorization-server\n    - https://newtqnia.com/.well-known/oauth-protected-resource\n\nkey_management:\n  where: NewTqnia account profile page\n  docs: https://newtqnia.com/en/connect\n  max_active_keys: 5\n  operations: [create, label, replace, revoke]\n  display: >-\n    The full key value is shown exactly once at creation - the provider states it must be\n    copied immediately.\n  rotation: Self-service replace and revoke at any time.\n  identity_binding: >-\n    Keys are personal and inherit the account's role. A reader key grants read-only,\n    single-locale access to published content; editors and administrators receive the\n    complete bilingual record and a content-drafting workflow.\n\nauthorization_model:\n  style: role-derived\n  roles:\n  - name: reader\n    grants: >-\n      Published content only, in one locale, as title + summary + canonical URL. Never\n      the full article\
  \ body. Cannot create, edit or publish.\n  - name: editor-administrator\n    grants: >-\n      Complete bilingual record including bodies, tags and citations, access to\n      unpublished drafts, and a content-drafting workflow.\n  note: >-\n    Permissions are attached to the ACCOUNT behind the key rather than selected per key,\n    so two keys held by one user are equivalent in power. The OAuth scope pair\n    (mcp:read / mcp:write) is the only place authorization is expressed as a\n    requestable value.\n\ngaps:\n- >-\n  The OpenAPI contract declares no securitySchemes and no security requirement - the\n  optional API key is a plain header parameter. A generator or agent reading the spec\n  alone cannot tell that an authenticated mode exists at all.\n- >-\n  No /.well-known/openid-configuration; OIDC discovery is not offered (OAuth 2.1\n  metadata only, which is correct for MCP).\n- No documented key expiry or automatic rotation policy; keys live until revoked.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newtqnia/refs/heads/main/authentication/newtqnia-authentication.yml
summary_line: 0 schemes
tags:
- News API
- News
- Technology
- Artificial Intelligence
- Cybersecurity
- Developer Tools
- Cloud Computing
- Media
- Publishing
- Bilingual
---
