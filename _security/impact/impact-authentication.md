---
api_key_in: []
api_specs:
- filename: impact-brand-account-v14-openapi.yml
  format: yaml
  label: Impact Brand API
  slug: brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-brand-account-v14-openapi.yml
- filename: impact-partner-account-v16-openapi.yml
  format: yaml
  label: Impact Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-partner-account-v16-openapi.yml
- filename: impact-agency-advertisers-v3-openapi.yml
  format: yaml
  label: Impact Agency API
  slug: agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-agency-advertisers-v3-openapi.yml
- filename: impact-brand-advocate-account-v13-openapi.yml
  format: yaml
  label: Impact Advocate API
  slug: advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-brand-advocate-account-v13-openapi.yml
auth_types: []
description: Every authentication mechanism impact.com publishes across its REST APIs, its Advocate APIs and its MCP server, with what each one is used for and where it is declared.
kind: authentication
layout: security
method: searched
name: Impact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impact declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Impact
provider_slug: impact
scheme_count: 5
schemes:
- applies_to:
  - Brand API v14
  - Partner API v16
  - Agency API v3
  - Advocate API v13
  declared_in_openapi: partially
  declared_in_openapi_note: Only the nine Advocate v13 documents declare a securitySchemes block. All 29 Brand v14, 26 Partner v16 and 5 Agency v3 documents omit securitySchemes and security entirely, so the auth requirement is invisible to any tool reading those specs.
  failure_status: 401
  header: 'Authorization: Basic base64(AccountSID:AuthToken)'
  id: basicAuth
  password: Auth Token
  scheme: basic
  transport: HTTPS only, port 443
  type: http
  username: Account SID
- applies_to:
  - Advocate API v13
  declared_in: openapi/impact-brand-advocate-*-v13-openapi.yml
  declared_in_openapi: true
  description: Tenant API key, for server-to-server interactions only.
  id: APIKey
  scheme: basic
  type: http
- applies_to:
  - Advocate API v13
  - Advocate Web SDK
  - Advocate Mobile SDKs
  declared_in_openapi: true
  description: Per-user JWT used by the Advocate Web and Mobile SDKs and by Open Endpoints in client-side contexts.
  id: UserJWT
  in: header
  name: X-SaaSquatch-User-Token
  type: apiKey
- applies_to:
  - MCP server
  - multi-customer applications
  authorization_endpoint: https://app.impact.com/oauth2/authorize
  grants:
  - authorization_code
  - client_credentials
  - refresh_token
  http_status: 200
  id: oauth2
  introspection_endpoint: https://app.impact.com/oauth2/introspect
  issuer: https://app.impact.com
  jwks_uri: https://app.impact.com/oauth2/jwks
  metadata:
    authorization_server: https://app.impact.com/.well-known/oauth-authorization-server
    openid_configuration: https://app.impact.com/.well-known/openid-configuration
    protected_resource: https://app.impact.com/.well-known/oauth-protected-resource
  pkce:
  - S256
  probed: '2026-08-13'
  protocol: OAuth 2.1
  revocation_endpoint: https://app.impact.com/oauth2/revoke
  scopes:
  - mcp:read
  - mcp:write
  - openid
  token_endpoint: https://app.impact.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: oauth2
  userinfo_endpoint: https://app.impact.com/oauth2/userinfo
- discovery: https://app.impact.com/.well-known/openid-configuration
  id: openIdConnect
  id_token_signing:
  - RS256
  issuer: https://app.impact.com
  note: OIDC discovery is served, but scopes_supported lists only openid - no profile or email - so the identity surface is minimal.
  scopes_supported:
  - openid
  subject_types:
  - public
  type: openIdConnect
slug: impact-authentication
source_filename: impact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Impact Authentication Profile\ndescription: Every authentication mechanism impact.com publishes across its REST APIs, its\n  Advocate APIs and its MCP server, with what each one is used for and where it is declared.\ngenerated: '2026-08-13'\nmethod: searched\nsource: https://integrations.impact.com/brand-api-reference/readme/authentication\ndocs:\n  authentication: https://integrations.impact.com/brand-api-reference/readme/authentication\n  create_api_key: https://integrations.impact.com/rest-apis/api-quick-start/create-an-api-key\n  quick_start: https://integrations.impact.com/rest-apis/api-quick-start\n  mcp: https://integrations.impact.com/ai-solutions/mcp-quick-start\nschemes:\n  - id: basicAuth\n    type: http\n    scheme: basic\n    applies_to: [Brand API v14, Partner API v16, Agency API v3, Advocate API v13]\n    username: Account SID\n    password: Auth Token\n    header: 'Authorization: Basic base64(AccountSID:AuthToken)'\n    transport: HTTPS only, port 443\n\
  \    declared_in_openapi: partially\n    declared_in_openapi_note: Only the nine Advocate v13 documents declare a securitySchemes\n      block. All 29 Brand v14, 26 Partner v16 and 5 Agency v3 documents omit securitySchemes\n      and security entirely, so the auth requirement is invisible to any tool reading those\n      specs.\n    failure_status: 401\n  - id: APIKey\n    type: http\n    scheme: basic\n    applies_to: [Advocate API v13]\n    description: Tenant API key, for server-to-server interactions only.\n    declared_in_openapi: true\n    declared_in: openapi/impact-brand-advocate-*-v13-openapi.yml\n  - id: UserJWT\n    type: apiKey\n    in: header\n    name: X-SaaSquatch-User-Token\n    applies_to: [Advocate API v13, Advocate Web SDK, Advocate Mobile SDKs]\n    description: Per-user JWT used by the Advocate Web and Mobile SDKs and by Open Endpoints in\n      client-side contexts.\n    declared_in_openapi: true\n  - id: oauth2\n    type: oauth2\n    applies_to: [MCP server, multi-customer\
  \ applications]\n    protocol: OAuth 2.1\n    issuer: https://app.impact.com\n    authorization_endpoint: https://app.impact.com/oauth2/authorize\n    token_endpoint: https://app.impact.com/oauth2/token\n    revocation_endpoint: https://app.impact.com/oauth2/revoke\n    introspection_endpoint: https://app.impact.com/oauth2/introspect\n    userinfo_endpoint: https://app.impact.com/oauth2/userinfo\n    jwks_uri: https://app.impact.com/oauth2/jwks\n    grants: [authorization_code, client_credentials, refresh_token]\n    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt,\n      private_key_jwt, none]\n    scopes: [mcp:read, mcp:write, openid]\n    metadata:\n      authorization_server: https://app.impact.com/.well-known/oauth-authorization-server\n      protected_resource: https://app.impact.com/.well-known/oauth-protected-resource\n      openid_configuration: https://app.impact.com/.well-known/openid-configuration\n    probed: '2026-08-13'\n\
  \    http_status: 200\n  - id: openIdConnect\n    type: openIdConnect\n    issuer: https://app.impact.com\n    discovery: https://app.impact.com/.well-known/openid-configuration\n    id_token_signing: [RS256]\n    subject_types: [public]\n    scopes_supported: [openid]\n    note: OIDC discovery is served, but scopes_supported lists only openid - no profile or\n      email - so the identity surface is minimal.\ntoken_model:\n  scoped_tokens:\n    available: true\n    since: April 2025\n    granularity: per API category and per endpoint\n    creation: impact.com UI, Settings, Technical, API, Create Access Token\n    forbidden_status: 403\n    note: A scoped token that is disabled, or enabled but not permitted on the endpoint,\n      returns 403 rather than 401.\n  legacy_tokens:\n    available: true\n    granularity: read/write or read-only only\n    status: supported, upgrade encouraged, no sunset date published\n  mcp_tokens:\n    minted_per: LLM client\n    scoped_to: the consenting user's\
  \ own platform permissions\n    refresh: refresh token issued\n    revocation: per-token delete in the UI, or account-wide MCP disable which deletes every\n      minted token\n  api_version_pinning: each token is created against a specific API version\nguidance_published:\n  - Start with read-only scopes so scripts cannot mutate production objects.\n  - Use separate tokens per environment (development, staging, production).\n  - Never hardcode credentials; use a vault or encrypted environment variables.\n  - Redact Account SID, Auth Token, OAuth and bearer tokens from anything pasted into\n    third-party assistants.\nfindings:\n  - Documentation-level auth is strong and explicit, but spec-level auth is largely missing -\n    60 of 69 published OpenAPI documents declare no security scheme at all.\n  - impact.com serves all three OAuth/OIDC discovery documents anonymously on app.impact.com,\n    which is unusual for a platform of this type and materially helps agent clients.\nprovider_action:\
  \ Add the documented basicAuth securityScheme and a top-level security\n  requirement to the Brand, Partner and Agency OpenAPI documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/authentication/impact-authentication.yml
summary_line: 5 schemes
tags:
- Affiliates
- Partnerships
- Performance Marketing
- Commission
- Tracking
- Creator Economy
- Partner Management
- Referral
- Attribution
- Payouts
- Marketing
- Advertising
- MCP
- Agents
---
