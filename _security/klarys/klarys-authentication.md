---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Klarys Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Klarys secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Klarys
provider_slug: klarys
scheme_count: 1
schemes:
- authorization_response_iss_parameter_supported: true
  client_id_metadata_document_supported: false
  code_challenge_methods:
  - S256
  endpoints:
    authorization: https://klarys.app/api/public/o/authorize/
    introspection: https://klarys.app/api/public/o/introspect/
    registration: https://klarys.app/api/public/o/register/
    revocation: https://klarys.app/api/public/o/revoke_token/
    token: https://klarys.app/api/public/o/token/
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  introspection_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  issuer: https://klarys.app/api/public/o
  name: OAuth2
  response_types:
  - code
  revocation_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  scopes:
  - groups
  - introspection
  - mcp:read
  - mcp:write
  - read
  - write
  scopes_artifact: scopes/klarys-scopes.yml
  sources:
  - well-known/klarys-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: klarys-authentication
source_filename: klarys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://klarys.app/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the RFC 8414 authorization-server metadata Klarys serves anonymously. There is no public\n  OpenAPI to derive securitySchemes from and no public authentication documentation page, so this profile\n  is built entirely from the machine-readable metadata document plus observed endpoint behaviour. Klarys\n  publishes no developer portal; the tenant login is at https://klarys.app/fr/accounts/login/.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  pkce: S256\n  dynamic_client_registration: true\n  token_introspection: true\n  token_revocation: true\n  openid_connect: false\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://klarys.app/api/public/o\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\n  grant_types:\n  - authorization_code\n  - client_credentials\n\
  \  - refresh_token\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  authorization_response_iss_parameter_supported: true\n  client_id_metadata_document_supported: false\n  endpoints:\n    authorization: https://klarys.app/api/public/o/authorize/\n    token: https://klarys.app/api/public/o/token/\n    revocation: https://klarys.app/api/public/o/revoke_token/\n    introspection: https://klarys.app/api/public/o/introspect/\n    registration: https://klarys.app/api/public/o/register/\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  revocation_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  introspection_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  scopes:\n  - groups\n  - introspection\n  - mcp:read\n  - mcp:write\n  - read\n  - write\n  scopes_artifact: scopes/klarys-scopes.yml\nendpoint_probes:\n- url: https://klarys.app/api/public/o/authorize/\n \
  \ method: GET\n  status: 302\n  note: redirects (missing client_id / unauthenticated) — endpoint is live\n- url: https://klarys.app/api/public/o/token/\n  method: GET\n  status: 405\n  note: method not allowed — POST-only token endpoint is live\n- url: https://klarys.app/api/public/o/register/\n  method: GET\n  status: 405\n  note: method not allowed — POST-only dynamic client registration endpoint is live\n- url: https://klarys.app/api/public/o/introspect/\n  method: GET\n  status: 403\n  note: forbidden without credentials — endpoint is live\n- url: https://klarys.app/api/schema/\n  method: GET\n  status: 401\n  note: 'schema endpoint exists but is customer-gated: {\"code\":1003,\"error\":\"User is unauthenticated\"}'\ngaps:\n- No public authentication documentation page.\n- No OpenID Connect discovery document (/.well-known/openid-configuration is 404), so the metadata\n  advertises OAuth 2.0 only, not OIDC.\n- No RFC 9728 protected-resource metadata, which is what an MCP client needs\
  \ to locate the\n  authorization server from a resource URL.\n- Scope descriptions are not published; only scope names are discoverable.\nx-evidence:\n  fetched: '2026-08-17'\n  url: https://klarys.app/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarys/refs/heads/main/authentication/klarys-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- SaaS
- eProcurement
- Procurement
- Supply Chain
- Food and Beverage
- Seafood
- Fresh Food
- Retail
- EDI
- Invoicing
- France
---
