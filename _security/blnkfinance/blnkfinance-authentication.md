---
api_key_in: []
api_specs:
- filename: blnkfinance-accounts-api-openapi.yml
  format: yaml
  label: Blnk Finance Accounts API
  slug: blnkfinance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-accounts-api-openapi.yml
- filename: blnkfinance-backup-api-openapi.yml
  format: yaml
  label: Blnk Finance Backup API
  slug: blnkfinance-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-backup-api-openapi.yml
- filename: blnkfinance-balance-monitors-api-openapi.yml
  format: yaml
  label: Blnk Finance Balance Monitors API
  slug: blnkfinance-balance-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-balance-monitors-api-openapi.yml
- filename: blnkfinance-balances-api-openapi.yml
  format: yaml
  label: Blnk Finance Balances API
  slug: blnkfinance-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-balances-api-openapi.yml
- filename: blnkfinance-identities-api-openapi.yml
  format: yaml
  label: Blnk Finance Identities API
  slug: blnkfinance-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-identities-api-openapi.yml
- filename: blnkfinance-ledgers-api-openapi.yml
  format: yaml
  label: Blnk Finance Ledgers API
  slug: blnkfinance-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-ledgers-api-openapi.yml
- filename: blnkfinance-refund-transaction-api-openapi.yml
  format: yaml
  label: Blnk Finance Refund Transaction API
  slug: blnkfinance-refund-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-refund-transaction-api-openapi.yml
- filename: blnkfinance-transactions-api-openapi.yml
  format: yaml
  label: Blnk Finance Transactions API
  slug: blnkfinance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/openapi/blnkfinance-transactions-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Blnkfinance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blnk Finance secures its APIs with apiKey, http, and oauth2 across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blnk Finance
provider_slug: blnkfinance
scheme_count: 0
schemes: []
slug: blnkfinance-authentication
source_filename: blnkfinance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.blnkfinance.com/advanced/configuration/server-security,\n  https://docs.blnkfinance.com/api-keys/overview, https://docs.blnkfinance.com/api-keys/scopes,\n  https://docs.blnkfinance.com/cloud/auth/api-keys, https://docs.blnkfinance.com/cloud/reference/mcp,\n  https://api.cloud.blnkfinance.com/.well-known/oauth-authorization-server (HTTP 200),\n  openapi/blnkfinance-core-openapi.json\nnote: >-\n  UPGRADED FROM DERIVED. The published OpenAPI declares a single securityScheme -- http/basic -- and\n  applies it nowhere. That is wrong about the shipped product: every documented Core call authenticates\n  with the X-Blnk-Key header, and Blnk Cloud uses Bearer with API keys or OAuth 2.0. The spec's\n  http/basic scheme is recorded below as spec_declares for provenance, but the surfaces[] block is what\n  an integrator should read.\nsummary:\n  types: [apiKey, http, oauth2]\n  primary: X-Blnk-Key header (Core), Bearer\
  \ token (Cloud)\nspec_declares:\n  file: openapi/blnkfinance-core-openapi.json\n  schemes:\n  - {name: basic, type: http, scheme: basic}\n  applied_to_operations: 0\n  discrepancy: >-\n    The spec neither declares the X-Blnk-Key apiKey scheme nor applies any security requirement to its\n    18 operations. Generated clients built from this spec will emit no auth header at all.\nsurfaces:\n- surface: Blnk Core REST API (self-hosted)\n  base: http://localhost:5001 (default; operator-chosen in production)\n  schemes:\n  - name: blnk-key\n    type: apiKey\n    in: header\n    header: X-Blnk-Key\n    accepts:\n    - kind: master key\n      value_source: BLNK_SERVER_SECRET_KEY\n      privileges: full access; the only key that can manage hooks or act across owners\n    - kind: scoped API key\n      value_source: created via the API key endpoints\n      privileges: 'resource:action scopes (see scopes/blnkfinance-scopes.yml)'\n      expiry: supported (expires_at)\n      owner_context: 'keys carry\
  \ an owner; non-master keys are confined to their own owner_id'\n      storage: hashed at rest since Core 0.12.0; encrypted with AES-256-GCM per the security page\n  enforcement_flag:\n    key: BLNK_SERVER_SECURE\n    default: false\n    behavior: >-\n      When false Blnk SKIPS authentication checks entirely. Authentication is only enforced when the\n      operator sets it to true, which the docs call out as a required step for \"any real deployment\".\n      This is the single most important thing an integrator must know about Blnk Core auth: the shipped\n      default is open.\n  errors:\n  - {code: AUTH_MISSING_API_KEY, status: 401}\n  - {code: AUTH_INVALID_API_KEY, status: 401}\n  - {code: AUTH_EXPIRED_API_KEY, status: 401}\n  - {code: AUTH_INSUFFICIENT_PERMISSIONS, status: 403}\n  - {code: AUTH_MASTER_KEY_REQUIRED, status: 403}\n  - {code: AUTH_CROSS_OWNER_ACCESS, status: 403}\n  - {code: AUTH_SCOPE_ESCALATION, status: 403}\n  docs: https://docs.blnkfinance.com/api-keys/overview\n\
  - surface: Blnk Cloud REST API\n  base: https://api.cloud.blnkfinance.com\n  schemes:\n  - name: bearer-api-key\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <api key>'\n    docs: https://docs.blnkfinance.com/cloud/auth/api-keys\n  - name: oauth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://api.cloud.blnkfinance.com/oauth/authorize\n        tokenUrl: https://api.cloud.blnkfinance.com/oauth/token\n        refreshUrl: https://api.cloud.blnkfinance.com/oauth/token\n        pkce: [S256, plain]\n    grant_types: [authorization_code, refresh_token]\n    client_auth: [client_secret_post, client_secret_basic]\n    metadata:\n      rfc8414: https://api.cloud.blnkfinance.com/.well-known/oauth-authorization-server\n      openid_configuration: https://api.cloud.blnkfinance.com/.well-known/openid-configuration\n      http_status: 200\n      probed: '2026-08-27'\n      note: >-\n        The two documents are byte-identical and neither\
  \ advertises an id_token, jwks_uri, userinfo\n        endpoint or scopes_supported -- so despite the /.well-known/openid-configuration path this is\n        plain OAuth 2.0 authorization-code, not OpenID Connect. Do not treat it as an OIDC provider.\n    docs: https://docs.blnkfinance.com/cloud/auth/oauth\n  unauthenticated_behavior:\n    status: 401\n    body: '{\"error\":\"Authorization header is required\"}'\n    note: Every path on api.cloud.blnkfinance.com returns this except the two OAuth metadata documents.\n- surface: Blnk Cloud MCP (ledger)\n  base: https://api.cloud.blnkfinance.com/mcp/{instance_id}\n  schemes:\n  - name: bearer\n    type: http\n    scheme: bearer\n    accepts: [Blnk Cloud API key, OAuth 2.0 access token]\n    required_scopes: ['mcp:read', 'mcp:write']\n  docs: https://docs.blnkfinance.com/cloud/reference/mcp\n- surface: Blnk docs MCP\n  base: https://docs.blnkfinance.com/mcp\n  schemes:\n  - {name: none, type: none}\n  note: Open, no authentication. Documentation\
  \ search only.\n- surface: Prometheus metrics\n  base: GET /metrics on the Core API port and worker monitoring port\n  schemes:\n  - name: metrics-bearer\n    type: http\n    scheme: bearer\n    value_source: BLNK_METRICS_BEARER_TOKEN\n  access_matrix:\n  - {secure: false, token_set: false, access: open}\n  - {secure: false, token_set: true, access: bearer required}\n  - {secure: true, token_set: true, access: bearer required}\n  - {secure: true, token_set: false, access: blocked}\n  docs: https://docs.blnkfinance.com/advanced/configuration/server-security#metrics-endpoint\nsecrets_note: >-\n  BLNK_SERVER_SECRET_KEY is BOTH the master API key and the HMAC signing secret for outgoing webhooks\n  and hook callbacks. Rotating it invalidates request auth and breaks webhook signature verification on\n  every receiver at the same time.\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blnkfinance/refs/heads/main/authentication/blnkfinance-authentication.yml
summary_line: apiKey/http/oauth2 · 0 schemes
tags:
- Fintech
- Financial-Services
- Ledger
- double-entry-accounting
- Payments
- Wallets
- Lending
- Banking Infrastructure
- Open-Source
- MCP
- AI Agents
- Developer Tools
---
