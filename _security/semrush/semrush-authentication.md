---
api_key_in: []
api_specs:
- filename: semrush-hermes-partner-api-api-openapi.yml
  format: yaml
  label: Semrush Hermes Partner API API
  slug: semrush-hermes-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-hermes-partner-api-api-openapi.yml
- filename: semrush-jwt-issuer-api-openapi.yml
  format: yaml
  label: Semrush JWT Issuer API
  slug: semrush-jwt-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-jwt-issuer-api-openapi.yml
- filename: semrush-partner-service-api-openapi.yml
  format: yaml
  label: Semrush Partner Service API
  slug: semrush-partner-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-partner-service-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: 'Authentication profile for the Semrush API surface. Upgrades the previous derived profile (which saw only the single bearer scheme in the App Center OpenAPI) with the three mechanisms Semrush actually documents: version-scoped API keys passed as a header or a query parameter, OAuth 2.0 with a device-authorization flow, and OAuth for the MCP server.'
kind: authentication
layout: security
method: searched
name: Semrush Authentication
name_suffix: Authentication
oauth_flows: []
overview: Semrush secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Semrush
provider_slug: semrush
scheme_count: 4
schemes:
- applies_to:
  - Backlinks API v4
  - Keywords API v4
  - Projects API v4
  - Listing Management API v4
  description: The recommended way to authorize a Version 4 request. Note the non-standard scheme token "Apikey" in the Authorization header — it is neither Bearer nor Basic, so generic HTTP clients and OpenAPI generators need it configured explicitly.
  in: header
  name: apiKeyHeader
  parameter: Authorization
  recommended: true
  source: https://developer.semrush.com/api/v4/get-started/authorization/
  type: apiKey
  value_format: Apikey <YOUR_API_KEY>
- applies_to:
  - Standard API v3 (Domain, Keyword, Overview, Subdomain, Subfolder, URL and Backlinks reports)
  - Trends API v3
  - API unit balance endpoint
  description: The v3 Standard API is a single query-string dispatcher; the credential travels in the URL. Semrush's own docs warn that the key also grants access to the account's API unit balance, so exposure carries a direct billing consequence.
  example: https://api.semrush.com/?key=<key>&type=domain_ranks&domain=apple.com&database=us
  in: query
  name: apiKeyQuery
  parameter: key
  risk: credential-in-url
  source: https://developer.semrush.com/api/v4/get-started/authorization/
  type: apiKey
- applies_to:
  - Map Rank Tracker API
  - Projects API (OAuth 2.0) — deprecated
  - Listing Management API (OAuth 2.0) — deprecated
  - Semrush MCP server
  flows:
  - description: The self-serve path — a developer signs in with their own Semrush account and stores the resulting tokens; no application to Semrush Support is needed. For multi-tenant apps the flow is repeated per tenant at setup.
    device_endpoint: https://oauth.semrush.com/dag/device/code
    name: Device Authorization Grant
    recommended: true
    returns:
    - device_code
    - user_code
    - verification_uri
    - expires_in
    - interval
    rfc: RFC 8628
  - description: The legacy path. Requires contacting Semrush Customer Support and waiting for issued credentials.
    name: Semrush Auth flow
    recommended: false
  - applies_to:
    - Semrush MCP
    description: Advertised in the RFC 8414 metadata at mcp.semrush.com — authorization_code and refresh_token grants, S256 and plain challenge methods, dynamic client registration, token_endpoint_auth_methods "none" (public clients).
    name: Authorization Code with PKCE
    rfc: RFC 7636
  name: oauth2Bearer
  parameter: Authorization
  scheme: bearer
  source: https://developer.semrush.com/api/v4/get-started/authorization/
  type: http
  value_format: Bearer <TOKEN>
- applies_to:
  - App Center Partner Service API
  - Hermes Partner API
  bearerFormat: JWT
  description: App Center server-to-server surface. A partner exchanges its credentials at POST /app-center-api/v2/jwt-token/ for a JWT, then presents it as a bearer token.
  name: jwtIssuerToken
  scheme: bearer
  sources:
  - openapi/_original/semrush-openapi.yml
  - https://www.semrush.com/apps/docs/server-to-server-api/bearer-token
  type: http
slug: semrush-authentication
source_filename: semrush-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.semrush.com/api/v4/get-started/authorization/\ndocs: https://developer.semrush.com/api/v4/get-started/authorization/\nprovider: Semrush\nproviderId: semrush\ndescription: >-\n  Authentication profile for the Semrush API surface. Upgrades the previous derived profile\n  (which saw only the single bearer scheme in the App Center OpenAPI) with the three\n  mechanisms Semrush actually documents: version-scoped API keys passed as a header or a\n  query parameter, OAuth 2.0 with a device-authorization flow, and OAuth for the MCP server.\n\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  primary: apiKey\n  mfa_on_api: false\n\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'Apikey <YOUR_API_KEY>'\n  recommended: true\n  applies_to:\n  - Backlinks API v4\n  - Keywords API v4\n  - Projects API v4\n  - Listing Management API v4\n  description: >-\n \
  \   The recommended way to authorize a Version 4 request. Note the non-standard scheme token\n    \"Apikey\" in the Authorization header — it is neither Bearer nor Basic, so generic HTTP\n    clients and OpenAPI generators need it configured explicitly.\n  source: https://developer.semrush.com/api/v4/get-started/authorization/\n\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  applies_to:\n  - Standard API v3 (Domain, Keyword, Overview, Subdomain, Subfolder, URL and Backlinks reports)\n  - Trends API v3\n  - API unit balance endpoint\n  example: 'https://api.semrush.com/?key=<key>&type=domain_ranks&domain=apple.com&database=us'\n  description: >-\n    The v3 Standard API is a single query-string dispatcher; the credential travels in the\n    URL. Semrush's own docs warn that the key also grants access to the account's API unit\n    balance, so exposure carries a direct billing consequence.\n  risk: credential-in-url\n  source: https://developer.semrush.com/api/v4/get-started/authorization/\n\
  \n- name: oauth2Bearer\n  type: http\n  scheme: bearer\n  parameter: Authorization\n  value_format: 'Bearer <TOKEN>'\n  applies_to:\n  - Map Rank Tracker API\n  - Projects API (OAuth 2.0) — deprecated\n  - Listing Management API (OAuth 2.0) — deprecated\n  - Semrush MCP server\n  flows:\n  - name: Device Authorization Grant\n    rfc: RFC 8628\n    recommended: true\n    device_endpoint: https://oauth.semrush.com/dag/device/code\n    returns: [device_code, user_code, verification_uri, expires_in, interval]\n    description: >-\n      The self-serve path — a developer signs in with their own Semrush account and stores\n      the resulting tokens; no application to Semrush Support is needed. For multi-tenant\n      apps the flow is repeated per tenant at setup.\n  - name: Semrush Auth flow\n    recommended: false\n    description: >-\n      The legacy path. Requires contacting Semrush Customer Support and waiting for issued\n      credentials.\n  - name: Authorization Code with PKCE\n   \
  \ rfc: RFC 7636\n    applies_to: [Semrush MCP]\n    description: >-\n      Advertised in the RFC 8414 metadata at mcp.semrush.com — authorization_code and\n      refresh_token grants, S256 and plain challenge methods, dynamic client registration,\n      token_endpoint_auth_methods \"none\" (public clients).\n  source: https://developer.semrush.com/api/v4/get-started/authorization/\n\n- name: jwtIssuerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to:\n  - App Center Partner Service API\n  - Hermes Partner API\n  description: >-\n    App Center server-to-server surface. A partner exchanges its credentials at\n    POST /app-center-api/v2/jwt-token/ for a JWT, then presents it as a bearer token.\n  sources:\n  - openapi/_original/semrush-openapi.yml\n  - https://www.semrush.com/apps/docs/server-to-server-api/bearer-token\n\nkey_management:\n  version_scoped: true\n  since: '2026-07-15'\n  v3:\n    count_per_account: 1\n    auto_generated: true\n    revocable: false\n\
  \    deletable: false\n    ttl: none\n    note: >-\n      A permanent, non-revocable credential. If a v3 key leaks there is no documented way to\n      rotate it — the account's only remedy is to contact Semrush.\n  v4:\n    max_per_account: 100\n    auto_generated_default: 1\n    revocable: true\n    deletable: true\n    renamable: true\n    ttl_configurable: true\n    permissions:\n    - Read-only (GET)\n    - Read and write (GET, POST, PUT, PATCH, DELETE)\n  visibility: >-\n    The full key value is displayed only once, at creation. Keys are managed in the API Keys\n    section of the Semrush user profile.\n\nwell_known:\n  oauth_authorization_server: https://mcp.semrush.com/.well-known/oauth-authorization-server\n  oauth_protected_resource: https://mcp.semrush.com/.well-known/oauth-protected-resource\n  openid_configuration: null\n  openid_connect: false\n\ngaps:\n- No mutual TLS, no signed requests, and no IP allow-listing documented.\n- No OpenID Connect — Semrush is not an identity\
  \ provider for third-party apps.\n- >-\n  The v3 credential cannot be rotated by the customer, while carrying direct spend authority\n  over the account's API unit balance.\n\ncross_links:\n  scopes: scopes/semrush-scopes.yml\n  conventions: conventions/semrush-conventions.yml\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/authentication/semrush-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Data
- Search Engines
- SEO
- Marketing
- Marketing Intelligence
- Content Marketing
- Advertising
- Competitive Intelligence
- Keyword Research
- Backlinks
- Rank Tracking
- AI Search Visibility
- Local SEO
- MCP
---
