---
api_key_in: []
api_specs:
- filename: sharethis-ai-summary-api-openapi.yml
  format: yaml
  label: ShareThis AI Summary API
  slug: sharethis-ai-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-ai-summary-api-openapi.yml
- filename: sharethis-apps-api-openapi.yml
  format: yaml
  label: ShareThis Apps API
  slug: sharethis-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-apps-api-openapi.yml
- filename: sharethis-audience-api-openapi.yml
  format: yaml
  label: ShareThis Audience API
  slug: sharethis-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-audience-api-openapi.yml
- filename: sharethis-authentication-api-openapi.yml
  format: yaml
  label: ShareThis Authentication API
  slug: sharethis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-authentication-api-openapi.yml
- filename: sharethis-oauth-clients-api-openapi.yml
  format: yaml
  label: ShareThis OAuth Clients API
  slug: sharethis-oauth-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-oauth-clients-api-openapi.yml
- filename: sharethis-properties-api-openapi.yml
  format: yaml
  label: ShareThis Properties API
  slug: sharethis-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-properties-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sharethis Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShareThis secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ShareThis
provider_slug: sharethis
scheme_count: 3
schemes:
- applied_to: All operations except POST /auth/login (13 of 14). Security is declared per-operation rather than by a global security requirement.
  bearerFormat: JWT
  credential_input: ShareThis account credentials
  expiry: not documented
  name: BearerToken
  obtain_via: POST https://platform-api.sharethis.com/v2.0/auth/login
  refresh: No refresh-token flow is documented for this surface; the contract exposes only the login exchange.
  scheme: bearer
  scopes: none
  sources:
  - openapi/sharethis-platform-api.json
  surface: ShareThis Platform API
  type: http
- authorization_endpoint: https://mcp.sharethis.com/oauth/authorize
  authorization_servers:
  - https://mcp.sharethis.com
  discovery_documents:
  - file: well-known/sharethis-mcp-oauth-protected-resource.json
    path: /.well-known/oauth-protected-resource
  - file: well-known/sharethis-mcp-oauth-authorization-server.json
    path: /.well-known/oauth-authorization-server
  - file: well-known/sharethis-mcp-openid-configuration.json
    path: /.well-known/openid-configuration
  grant_types:
  - authorization_code
  - client_credentials
  issuer: https://mcp.sharethis.com
  name: OAuth2 (MCP)
  pkce:
    required_methods:
    - S256
  prerequisite: A ShareThis account must exist at https://platform.sharethis.com before OAuth linking succeeds.
  resource: https://mcp.sharethis.com
  response_types:
  - code
  scopes:
  - description: Invoke MCP tools on the ShareThis MCP server. The only scope the authorization server advertises.
    name: mcp:tools
  sources:
  - https://mcp.sharethis.com/.well-known/oauth-authorization-server
  - https://mcp.sharethis.com/
  spec: OAuth 2.1 with RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata
  surface: ShareThis MCP Server
  token_endpoint: https://mcp.sharethis.com/oauth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  type: oauth2
- name: OAuth client management
  note: The Platform API also exposes POST/GET /oauth-clients and DELETE /oauth-clients/{client_id}, letting an account mint and revoke its own OAuth clients. Client creation is quota-limited (403 OAUTH_CLIENT_LIMIT_EXCEEDED); the numeric limit is not published.
  surface: ShareThis Platform API
  type: provisioning
slug: sharethis-authentication
source_filename: sharethis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  openapi/sharethis-platform-api.json (securitySchemes), https://sharethis.com/platform-api/,\n  https://mcp.sharethis.com/ and the live OAuth metadata at\n  https://mcp.sharethis.com/.well-known/oauth-authorization-server (probed 2026-08-27)\nsummary:\n  types:\n  - http\n  - oauth2\n  note: >-\n    ShareThis runs TWO different auth models across one product. The REST Platform API uses a\n    bearer JWT minted by its own login endpoint; the MCP server uses OAuth 2.1 authorization-code\n    with PKCE. They are not interchangeable — a Platform API token will not authorize an MCP call.\nschemes:\n- name: BearerToken\n  surface: ShareThis Platform API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  obtain_via: 'POST https://platform-api.sharethis.com/v2.0/auth/login'\n  credential_input: ShareThis account credentials\n  applied_to: >-\n    All operations except POST /auth/login (13 of 14). Security is declared per-operation\
  \ rather\n    than by a global security requirement.\n  scopes: none\n  expiry: not documented\n  refresh: >-\n    No refresh-token flow is documented for this surface; the contract exposes only the login\n    exchange.\n  sources:\n  - openapi/sharethis-platform-api.json\n- name: OAuth2 (MCP)\n  surface: ShareThis MCP Server\n  type: oauth2\n  spec: OAuth 2.1 with RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata\n  issuer: https://mcp.sharethis.com\n  authorization_endpoint: https://mcp.sharethis.com/oauth/authorize\n  token_endpoint: https://mcp.sharethis.com/oauth/token\n  grant_types:\n  - authorization_code\n  - client_credentials\n  response_types:\n  - code\n  pkce:\n    required_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  scopes:\n  - name: mcp:tools\n    description: >-\n      Invoke MCP tools on the ShareThis MCP server. The only scope the authorization server\n      advertises.\n  resource: https://mcp.sharethis.com\n\
  \  authorization_servers:\n  - https://mcp.sharethis.com\n  discovery_documents:\n  - path: /.well-known/oauth-protected-resource\n    file: well-known/sharethis-mcp-oauth-protected-resource.json\n  - path: /.well-known/oauth-authorization-server\n    file: well-known/sharethis-mcp-oauth-authorization-server.json\n  - path: /.well-known/openid-configuration\n    file: well-known/sharethis-mcp-openid-configuration.json\n  prerequisite: >-\n    A ShareThis account must exist at https://platform.sharethis.com before OAuth linking succeeds.\n  sources:\n  - https://mcp.sharethis.com/.well-known/oauth-authorization-server\n  - https://mcp.sharethis.com/\n- name: OAuth client management\n  surface: ShareThis Platform API\n  type: provisioning\n  note: >-\n    The Platform API also exposes POST/GET /oauth-clients and DELETE /oauth-clients/{client_id},\n    letting an account mint and revoke its own OAuth clients. Client creation is quota-limited\n    (403 OAUTH_CLIENT_LIMIT_EXCEEDED); the numeric\
  \ limit is not published.\nunauthenticated_surface:\n- api: ShareThis Social Share Count API\n  base_url: https://count-server.sharethis.com/v2.0\n  auth: none\n  verified: >-\n    Live GET of /get_counts?url=https://www.sharethis.com returned HTTP 200 with a full counts\n    payload and no credential of any kind (probed 2026-08-27).\n  note: >-\n    Genuinely open. This is the surface an agent can call today with zero onboarding, and the only\n    ShareThis API that needs no account.\n- surface: MCP tools/list discovery\n  auth: none\n  note: >-\n    tools/list on https://mcp.sharethis.com responds anonymously with complete input and output\n    schemas. Discovery is open; invocation is not.\nopenid_connect:\n  present: false\n  note: >-\n    An /.well-known/openid-configuration document IS served on mcp.sharethis.com, but it is an\n    OAuth authorization-server document wearing the OIDC filename — it advertises no id_token,\n    no userinfo_endpoint, no jwks_uri and no OIDC response\
  \ types. It should not be read as an\n    OpenID Connect provider.\nmutual_tls: false\napi_keys: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/authentication/sharethis-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Social Sharing
- Website Tools
- Audience Data
- Advertising Technology
- Analytics
- Consent Management
- Publishing
- MCP
---
