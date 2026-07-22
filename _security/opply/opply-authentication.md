---
api_key_in:
- cookie
- header
api_specs:
- filename: opply-openapi-original.yml
  format: yaml
  label: Opply API
  slug: opply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/openapi/opply-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Opply Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Opply secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Opply
provider_slug: opply
scheme_count: 3
schemes:
- description: 'Token-based authentication with the required prefix "Token" (e.g. `Authorization: Token <key>`).'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/opply-openapi-original.yml
  type: apiKey
- description: Django session cookie for first-party web app calls.
  in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/opply-openapi-original.yml
  type: apiKey
- description: 'OAuth 2.1 authorization server advertised via RFC 8414 metadata. Supports the authorization_code grant with PKCE (S256) and refresh_token, dynamic client registration (RFC 7591), and RFC 9728 protected-resource metadata for the MCP surface. Bearer access tokens are supplied in the Authorization header. token_endpoint_auth_methods: client_secret_post, client_secret_basic, none.'
  flows:
  - authorizationUrl: https://api.opply.com/api/v1/oauth/authorize/
    flow: authorizationCode
    registrationUrl: https://api.opply.com/api/v1/oauth/register/
    revocationUrl: https://api.opply.com/api/v1/oauth/revoke_token/
    scope_count: 29
    tokenUrl: https://api.opply.com/api/v1/oauth/token/
  name: OAuth2
  sources:
  - https://api.opply.com/.well-known/oauth-authorization-server
  type: oauth2
slug: opply-authentication
source_filename: opply-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/opply-openapi-original.yml\ndocs: https://api.opply.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Token-based authentication with the required prefix \"Token\"\n    (e.g. `Authorization: Token <key>`).\n  sources:\n  - openapi/opply-openapi-original.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  description: Django session cookie for first-party web app calls.\n  sources:\n  - openapi/opply-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization server advertised via RFC 8414 metadata. Supports\n    the authorization_code grant with PKCE (S256) and refresh_token, dynamic\n    client registration (RFC 7591), and\
  \ RFC 9728 protected-resource metadata for\n    the MCP surface. Bearer access tokens are supplied in the Authorization\n    header. token_endpoint_auth_methods: client_secret_post, client_secret_basic,\n    none.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.opply.com/api/v1/oauth/authorize/\n    tokenUrl: https://api.opply.com/api/v1/oauth/token/\n    revocationUrl: https://api.opply.com/api/v1/oauth/revoke_token/\n    registrationUrl: https://api.opply.com/api/v1/oauth/register/\n    scope_count: 29\n  sources:\n  - https://api.opply.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/authentication/opply-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Food and Beverage
- Supply Chain
- Procurement
- Ordering
- Payments
- Sourcing
- Logistics
- AI Agents
- MCP
---
