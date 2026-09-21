---
anonymous_access: true
api_key_in: []
api_specs:
- filename: agentdisco-io-openapi.yml
  format: yaml
  label: Agent Disco API
  slug: agent-disco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentdisco-io/refs/heads/main/openapi/agentdisco-io-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentdisco Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Disco declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Disco
provider_slug: agentdisco-io
scheme_count: 3
schemes:
- applies_to:
    optional:
    - post_api_scan_create
    - post_api_website_rescan
    required_account_bound:
    - get_api_key_list
    - delete_api_key_revoke
    - get_api_webhook_list
    - post_api_webhook_create
    - delete_api_webhook_delete
  bearer_format: ak_ token (first 10 chars, e.g. ak_XXXXXXX, are the loggable tokenPrefix)
  declared_in_spec: false
  header: 'Authorization: Bearer ak_...'
  id: bearerApiKey
  obtain:
  - detail: POST /api/v1/keys with no credential ("No account, no email - just click the button"); optional {label}; 201 returns the plaintext token ONCE plus id, tokenPrefix, rateLimitTier anonymous; 5 mints/hour per IP.
    method: anonymous mint
    operation: post_api_key_create
  - detail: Keys created from /account are bound to the account (rateLimitTier authenticated); the account activity log records key and webhook creation.
    method: website sign-in
    url: https://agentdisco.io/register
  - detail: See colony_token_exchange below; returns an account-bound authenticated-tier key.
    method: Colony agent sign-in
    operation: post_api_colony_agent_login
  revocation: DELETE /api/v1/keys/{id} - idempotent, immediate; a revoked key drops to the anonymous limit; you may revoke the key you authenticate with.
  scheme: bearer
  storage: The server keeps only a hash; plaintext is never returned after mint (GET /api/v1/keys shows tokenPrefix only).
  tiers:
  - quota: 10 scans/day per IP
    tier: anonymous (no key)
  - note: cannot own webhooks or list keys - 401 "Anonymous keys can't own webhooks"
    quota: 100 scans/day per key
    tier: anonymous key
  - quota: 500 scans/day per key
    tier: authenticated (account-bound key)
  type: http
- applies_to:
  - get_api_ops_check_health
  - get_api_ops_version
  declared_in_spec: referenced by two operations but undefined (components.securitySchemes is null)
  detail: 'Operator-only; credentials are the deployment''s OPS_BASIC_AUTH_USER / OPS_BASIC_AUTH_PASS env vars, not issued to API consumers. Observed: 401 with WWW-Authenticate: Basic realm="ops".'
  id: opsBasic
  realm: ops
  scheme: basic
  type: http
- applies_to:
  - get_openapi_spec
  - get_api_checks_index
  - get_api_scan_show
  - get_api_scan_diff
  - get_api_website_show
  - get_api_website_scans
  - get_api_website_badge
  - get_api_website_badge_png
  - get_api_colony_agent_login_discovery
  - post_api_key_create
  - post_api_website_unlist_request
  - post_api_website_unlist_confirm
  - post_api_website_relist_request
  - post_api_website_relist_confirm
  - delete_api_website_delete
  detail: Public reads, key mint, the DNS-TXT-verified unlist/relist flow and the right-to-delete endpoint are unauthenticated and rate-limited per IP.
  id: none
  type: none
slug: agentdisco-io-authentication
source_filename: agentdisco-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://agentdisco.io/developers\nsource: >-\n  https://agentdisco.io/developers, https://agentdisco.io/llms.txt, the operation descriptions in\n  openapi/agentdisco-io-openapi.yml (harvested from https://agentdisco.io/api/v1/openapi.json - whose\n  components.securitySchemes is null, which is why derive-authentication.py produced nothing), GET\n  https://agentdisco.io/api/v1/auth/colony/agent (200, observed 2026-09-19), the 401 bodies observed on\n  GET /api/v1/webhooks, /api/v1/keys and /api/v1/ops/version, and\n  https://thecolony.ai/.well-known/openid-configuration.\nsummary: >-\n  Bearer API keys (prefix ak_) with three quota tiers, obtainable three ways - anonymously with one POST,\n  by signing in on the website, or non-interactively by an autonomous agent presenting an RFC 8693 id_token\n  minted at The Colony. Most reads and scan submission need no credential at all. There is no OAuth\n  authorization server on agentdisco.io\
  \ itself; the Colony is a third-party issuer and Agent Disco is a\n  relying party. Two operator endpoints use HTTP Basic.\nschemes:\n- id: bearerApiKey\n  type: http\n  scheme: bearer\n  bearer_format: 'ak_ token (first 10 chars, e.g. ak_XXXXXXX, are the loggable tokenPrefix)'\n  header: 'Authorization: Bearer ak_...'\n  declared_in_spec: false\n  applies_to:\n    optional: [post_api_scan_create, post_api_website_rescan]\n    required_account_bound: [get_api_key_list, delete_api_key_revoke, get_api_webhook_list, post_api_webhook_create, delete_api_webhook_delete]\n  obtain:\n  - method: anonymous mint\n    operation: post_api_key_create\n    detail: 'POST /api/v1/keys with no credential (\"No account, no email - just click the button\"); optional {label}; 201 returns the plaintext token ONCE plus id, tokenPrefix, rateLimitTier anonymous; 5 mints/hour per IP.'\n  - method: website sign-in\n    url: https://agentdisco.io/register\n    detail: Keys created from /account are bound to the\
  \ account (rateLimitTier authenticated); the account activity log records key and webhook creation.\n  - method: Colony agent sign-in\n    operation: post_api_colony_agent_login\n    detail: See colony_token_exchange below; returns an account-bound authenticated-tier key.\n  tiers:\n  - {tier: anonymous (no key), quota: 10 scans/day per IP}\n  - {tier: anonymous key, quota: 100 scans/day per key, note: cannot own webhooks or list keys - 401 \"Anonymous keys can't own webhooks\"}\n  - {tier: authenticated (account-bound key), quota: 500 scans/day per key}\n  revocation: DELETE /api/v1/keys/{id} - idempotent, immediate; a revoked key drops to the anonymous limit; you may revoke the key you authenticate with.\n  storage: The server keeps only a hash; plaintext is never returned after mint (GET /api/v1/keys shows tokenPrefix only).\n- id: opsBasic\n  type: http\n  scheme: basic\n  realm: ops\n  declared_in_spec: referenced by two operations but undefined (components.securitySchemes is null)\n\
  \  applies_to: [get_api_ops_check_health, get_api_ops_version]\n  detail: 'Operator-only; credentials are the deployment''s OPS_BASIC_AUTH_USER / OPS_BASIC_AUTH_PASS env vars, not issued to API consumers. Observed: 401 with WWW-Authenticate: Basic realm=\"ops\".'\n- id: none\n  type: none\n  applies_to: [get_openapi_spec, get_api_checks_index, get_api_scan_show, get_api_scan_diff, get_api_website_show, get_api_website_scans, get_api_website_badge, get_api_website_badge_png, get_api_colony_agent_login_discovery, post_api_key_create, post_api_website_unlist_request, post_api_website_unlist_confirm, post_api_website_relist_request, post_api_website_relist_confirm, delete_api_website_delete]\n  detail: Public reads, key mint, the DNS-TXT-verified unlist/relist flow and the right-to-delete endpoint are unauthenticated and rate-limited per IP.\ncolony_token_exchange:\n  standard: OAuth 2.0 Token Exchange (RFC 8693)\n  role_of_agentdisco: relying party / audience\n  issuer: https://thecolony.ai\n\
  \  token_endpoint: https://thecolony.ai/oauth/token\n  audience: colony_gNvs-06hD2sPmBWHgQ4skwGUMpDwqmcl\n  grant_type: urn:ietf:params:oauth:grant-type:token-exchange\n  subject_token_type: urn:ietf:params:oauth:token-type:access_token\n  requested_token_type: urn:ietf:params:oauth:token-type:id_token\n  scope: openid profile\n  discovery: GET https://agentdisco.io/api/v1/auth/colony/agent (get_api_colony_agent_login_discovery) publishes all of the above; cacheable, static per deployment.\n  exchange_endpoint: 'POST https://agentdisco.io/api/v1/auth/colony/agent with {\"id_token\": \"...\"}'\n  responses:\n    201: authenticated-tier ak_ key shown once\n    400: missing id_token\n    401: invalid/expired token, wrong audience, or a non-agent (human) subject\n    404: Colony login disabled on this deployment\n    429: too many attempts from this IP\n  rules:\n  - Only an id_token audienced to AgentDisco is accepted; never send the raw Colony credential.\n  - Agent-only - human Colony subjects\
  \ are rejected; humans use \"Log in with the Colony\" on the website.\n  - The Python SDK (>=0.4.0) runs the exchange at the Colony itself (AgentDisco.from_colony_token).\n  colony_metadata:\n    file: well-known/agentdisco-io-colony-openid-configuration.json\n    registration_endpoint: https://thecolony.ai/oauth/register\n    pkce: S256\n    grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:token-exchange', 'urn:openid:params:grant-type:ciba', 'urn:ietf:params:oauth:grant-type:device_code']\nown_oauth_metadata:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  note: Agent Disco publishes no RFC 8414 / RFC 9728 / OIDC discovery of its own; it issues opaque ak_ keys, not OAuth tokens.\ndelegated_identity:\n  supported: true\n  mechanism: Colony identity -> RFC 8693 token exchange -> account-bound ak_ key\n  human_in_loop: none required for agents holding a Colony identity\nwebsite_accounts:\n  sign_up:\
  \ https://agentdisco.io/register\n  login: https://agentdisco.io/login\n  detail: Password accounts with optional 2FA and a per-user activity log at /account/activity (privacy policy section 2); \"Log in with the Colony\" is offered to humans.\nrelated:\n  conventions: conventions/agentdisco-io-conventions.yml\n  rate_limits: rate-limits/agentdisco-io-rate-limits.yml\n  overlay_adding_securitySchemes: overlays/agentdisco-io-openapi-overlay.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentdisco-io/refs/heads/main/authentication/agentdisco-io-authentication.yml
summary_line: 3 schemes
tags:
- AI Agents
- Agent Discoverability
- Website Auditing
- Developer Tools
- Webhook
- llms-txt
- A2A
- MCP
- Scanning
---
