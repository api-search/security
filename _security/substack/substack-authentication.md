---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: probed
name: Substack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- implicit
- refreshToken
overview: Substack secures its APIs with oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, implicit, and refreshToken flow(s).
provider_name: Substack
provider_slug: substack
scheme_count: 4
schemes:
- authorization_response_iss_parameter_supported: true
  endpoints:
    end_session: https://substack.com/oauth/session/end
    jwks: https://substack.com/oauth/jwks
    pushed_authorization_request: https://substack.com/oauth/request
    registration: https://substack.com/oauth/register
    userinfo: https://substack.com/oauth/me
  flows:
    authorizationCode:
      authorizationUrl: https://substack.com/oauth/auth
      pkce_methods:
      - S256
      refreshUrl: https://substack.com/oauth/token
      scope_count: 8
      tokenUrl: https://substack.com/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://substack.com/oauth/device/auth
      grant: urn:ietf:params:oauth:grant-type:device_code
      tokenUrl: https://substack.com/oauth/token
    implicit:
      authorizationUrl: https://substack.com/oauth/auth
      note: advertised in the OIDC document only
  id_token_signing_algs:
  - PS256
  - RS256
  issuer: https://substack.com
  name: SubstackOAuth
  response_modes:
  - form_post
  - fragment
  - query
  response_types:
  - code id_token
  - code
  - id_token
  - none
  scopes_source: scopes/substack-scopes.yml
  surfaces:
  - mcp.substack.com/api/v1/mcp
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  type: oauth2
- claims:
  - sub
  - name
  - subscription
  - publication_role
  - email
  - publication_id
  - sid
  - auth_time
  - iss
  name: SubstackOIDC
  note: Non-canonical discovery location. The RFC 8615 path https://substack.com/.well-known/openid-configuration returns 404; a client that follows the spec will not find this document.
  openIdConnectUrl: https://substack.com/oauth/.well-known/openid-configuration
  type: openIdConnect
- challenge: Bearer realm="substack", resource_metadata="https://mcp.substack.com/.well-known/oauth-protected-resource/api/v1/mcp"
  in: header
  name: MCPBearer
  parameter: Authorization
  protected_resource_metadata: https://mcp.substack.com/.well-known/oauth-protected-resource/api/v1/mcp
  required_scope: mcp:read
  scheme: bearer
  surface: https://mcp.substack.com/api/v1/mcp
  type: http
- docs: https://support.substack.com/hc/en-us/articles/45099095296916-Substack-Developer-API
  in: header
  issuance: Create a Substack account, accept the Developer API Terms of Use, submit the access form, then generate a token under Settings > Developer API > Create new token. Substack states access is granted within 7-10 business days to applicants who meet its requirements.
  name: DeveloperAPIToken
  note: The technical documentation article is linked from Substack's own API Terms of Use but is not listed in the public Help Center index and its Zendesk API record returns 401, so the exact header name and error contract could not be read first-party. Not recorded rather than guessed.
  parameter: Authorization
  scheme: bearer
  surface: https://substack.com
  terms: https://substack.com/api-tos
  type: http
slug: substack-authentication
source_filename: substack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://substack.com/.well-known/oauth-authorization-server,\n  https://substack.com/oauth/.well-known/openid-configuration,\n  https://mcp.substack.com/.well-known/oauth-protected-resource/api/v1/mcp\ndocs: https://support.substack.com/hc/en-us/articles/45099095296916-Substack-Developer-API\nnote: >-\n  Substack has no OpenAPI, so this profile was not derived from a spec — it was read\n  from the provider's live OAuth/OIDC discovery documents and from the WWW-Authenticate\n  challenge the MCP endpoint returns. Two distinct auth models are in play and they do\n  not share credentials: the Developer API uses a self-service bearer token minted in\n  account settings after an approval process, while the MCP server uses full OAuth 2.1\n  with dynamic client registration.\nsummary:\n  types: [oauth2, openIdConnect, http]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, deviceCode, implicit, refreshToken]\n  pkce:\
  \ [S256]\n  dynamic_client_registration: true\n  mtls: false\nschemes:\n  - name: SubstackOAuth\n    type: oauth2\n    issuer: https://substack.com\n    surfaces: [mcp.substack.com/api/v1/mcp]\n    flows:\n      authorizationCode:\n        authorizationUrl: https://substack.com/oauth/auth\n        tokenUrl: https://substack.com/oauth/token\n        refreshUrl: https://substack.com/oauth/token\n        pkce_methods: [S256]\n        scope_count: 8\n      deviceCode:\n        deviceAuthorizationUrl: https://substack.com/oauth/device/auth\n        tokenUrl: https://substack.com/oauth/token\n        grant: urn:ietf:params:oauth:grant-type:device_code\n      implicit:\n        authorizationUrl: https://substack.com/oauth/auth\n        note: advertised in the OIDC document only\n    endpoints:\n      registration: https://substack.com/oauth/register\n      jwks: https://substack.com/oauth/jwks\n      userinfo: https://substack.com/oauth/me\n      pushed_authorization_request: https://substack.com/oauth/request\n\
  \      end_session: https://substack.com/oauth/session/end\n    token_endpoint_auth_methods: [none, client_secret_basic]\n    id_token_signing_algs: [PS256, RS256]\n    response_types: ['code id_token', code, id_token, none]\n    response_modes: [form_post, fragment, query]\n    authorization_response_iss_parameter_supported: true\n    scopes_source: scopes/substack-scopes.yml\n  - name: SubstackOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://substack.com/oauth/.well-known/openid-configuration\n    note: >-\n      Non-canonical discovery location. The RFC 8615 path\n      https://substack.com/.well-known/openid-configuration returns 404; a client that\n      follows the spec will not find this document.\n    claims: [sub, name, subscription, publication_role, email, publication_id, sid, auth_time, iss]\n  - name: MCPBearer\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    surface: https://mcp.substack.com/api/v1/mcp\n    required_scope:\
  \ mcp:read\n    challenge: 'Bearer realm=\"substack\", resource_metadata=\"https://mcp.substack.com/.well-known/oauth-protected-resource/api/v1/mcp\"'\n    protected_resource_metadata: https://mcp.substack.com/.well-known/oauth-protected-resource/api/v1/mcp\n  - name: DeveloperAPIToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    surface: https://substack.com\n    issuance: >-\n      Create a Substack account, accept the Developer API Terms of Use, submit the\n      access form, then generate a token under Settings > Developer API > Create new\n      token. Substack states access is granted within 7-10 business days to applicants\n      who meet its requirements.\n    terms: https://substack.com/api-tos\n    docs: https://support.substack.com/hc/en-us/articles/45099095296916-Substack-Developer-API\n    note: >-\n      The technical documentation article is linked from Substack's own API Terms of\n      Use but is not listed in the public Help Center\
  \ index and its Zendesk API record\n      returns 401, so the exact header name and error contract could not be read\n      first-party. Not recorded rather than guessed.\nunauthenticated_surfaces:\n  - surface: https://{publication}.substack.com/feed\n    auth: none\n    note: public per-publication RSS; no credential required\n  - surface: https://{publication}.substack.com/api/v1/posts\n    auth: none\n    note: >-\n      Undocumented JSON endpoint used by the Substack web application. Reachable\n      anonymously and returns 200, but Substack publishes no contract for it and it is\n      not covered by the Developer API Terms of Use. Recorded as observed, not endorsed.\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://substack.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://substack.com/oauth/jwks\n    http_status: 200\n    content_type: application/jwk-set+json\n  - fetched: '2026-08-13'\n    url: https://mcp.substack.com/api/v1/mcp\n\
  \    http_status: 401\n  - fetched: '2026-08-13'\n    url: https://substack.com/api-tos\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/substack/refs/heads/main/authentication/substack-authentication.yml
summary_line: oauth2/openIdConnect/http · 4 schemes
tags:
- Newsletters
- Publishing
- Creator Economy
- Subscriptions
- Email
- Podcasting
- Notes
- Media
- Independent Media
- Paid Content
- MCP
- Agents
- RSS
- Analytics
---
