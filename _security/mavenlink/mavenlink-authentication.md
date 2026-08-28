---
api_key_in:
- header
api_specs:
- filename: mavenlink-openapi.yml
  format: yaml
  label: Kantata OX API
  slug: kantata-ox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenlink/refs/heads/main/openapi/mavenlink-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Mavenlink Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Mavenlink secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Mavenlink
provider_slug: mavenlink
scheme_count: 3
schemes:
- description: 'Swagger 2.0 models the bearer token as an apiKey header named "Bearer". In practice the header is `Authorization: Bearer <token>` as documented in the API reference; the securityDefinition name is an artifact of Swagger 2.0 having no native bearer type.'
  in: header
  name: BearerToken
  parameter: Bearer
  sources:
  - openapi/mavenlink-openapi.yml
  - https://developer.kantata.com/
  type: apiKey
- flows:
  - authorizationUrl: https://app.mavenlink.com/oauth/authorize
    flow: authorizationCode
    note: The spec declares an empty scopes map. The real scope list is published anonymously in the discovery documents - see scopes/mavenlink-scopes.yml.
    scopes: 0
    tokenUrl: https://app.mavenlink.com/oauth/token
  name: OauthSecurity
  sources:
  - openapi/mavenlink-openapi.yml
  type: oauth2
- authorization_endpoint: https://api.mavenlink.com/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - email
  - name
  - given_name
  - family_name
  - preferred_username
  - account_id
  - account_name
  code_challenge_methods_supported:
  - plain
  - S256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://api.mavenlink.com/oauth/introspect
  issuer: https://app.mavenlink.com
  jwks_uri: https://api.mavenlink.com/openid/discovery/keys
  name: KantataOpenIDConnect
  openIdConnectUrl: https://api.mavenlink.com/.well-known/openid-configuration
  revocation_endpoint: https://api.mavenlink.com/oauth/revoke
  sources:
  - well-known/mavenlink-api-openid-configuration.json
  - well-known/mavenlink-app-openid-configuration.json
  token_endpoint: https://api.mavenlink.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://api.mavenlink.com/openid/userinfo
slug: mavenlink-authentication
source_filename: mavenlink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://developer.kantata.com/ (Authentication section) + https://api.mavenlink.com/.well-known/openid-configuration\ndocs: https://developer.kantata.com/\nnotes: >-\n  Derived from the Swagger 2.0 securityDefinitions in openapi/mavenlink-openapi.yml, then upgraded from the\n  Kantata OX API documentation Authentication section and from the OpenID Connect / OAuth 2.0 discovery documents\n  that api.mavenlink.com and app.mavenlink.com serve anonymously (both probed 2026-08-25, HTTP 200).\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  primary: OAuth 2.0 authorization-code bearer token\n  anonymous_access: false\n  registration_required: true\n  registration_note: >-\n    Applications must be registered by a Kantata OX account administrator at\n    https://app.mavenlink.com/oauth/applications, and a paid\
  \ Kantata OX account is required to register one.\n    There is no self-serve developer sandbox.\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Bearer\n  description: >-\n    Swagger 2.0 models the bearer token as an apiKey header named \"Bearer\". In practice the header is\n    `Authorization: Bearer <token>` as documented in the API reference; the securityDefinition name is an\n    artifact of Swagger 2.0 having no native bearer type.\n  sources:\n  - openapi/mavenlink-openapi.yml\n  - https://developer.kantata.com/\n- name: OauthSecurity\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.mavenlink.com/oauth/authorize\n    tokenUrl: https://app.mavenlink.com/oauth/token\n    scopes: 0\n    note: >-\n      The spec declares an empty scopes map. The real scope list is published anonymously in the discovery\n      documents - see scopes/mavenlink-scopes.yml.\n  sources:\n  - openapi/mavenlink-openapi.yml\n- name: KantataOpenIDConnect\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://api.mavenlink.com/.well-known/openid-configuration\n  issuer: https://app.mavenlink.com\n  authorization_endpoint: https://api.mavenlink.com/oauth/authorize\n  token_endpoint: https://api.mavenlink.com/oauth/token\n  revocation_endpoint: https://api.mavenlink.com/oauth/revoke\n  introspection_endpoint: https://api.mavenlink.com/oauth/introspect\n  userinfo_endpoint: https://api.mavenlink.com/openid/userinfo\n  jwks_uri: https://api.mavenlink.com/openid/discovery/keys\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - email\n  - name\n  - given_name\n  - family_name\n  - preferred_username\n  - account_id\n  - account_name\n \
  \ sources:\n  - well-known/mavenlink-api-openid-configuration.json\n  - well-known/mavenlink-app-openid-configuration.json\ntoken_handling:\n  expiry: >-\n    The API reference states that Kantata OX OAuth access tokens do not expire and must be protected like\n    passwords. Revoking the application's access invalidates the token.\n  revocation: https://api.mavenlink.com/oauth/revoke\n  refresh: refresh_token grant is advertised in the OIDC discovery document\n  transport: HTTPS only; the API reference requires all requests be made over SSL\nmcp_authorization:\n  resource: https://api.mavenlink.com/mcp\n  protected_resource_metadata: https://api.mavenlink.com/.well-known/oauth-protected-resource\n  authorization_server: https://api.mavenlink.com\n  authorization_server_metadata: https://api.mavenlink.com/.well-known/oauth-authorization-server\n  bearer_methods_supported:\n  - header\n  scopes_supported:\n  - mcp\n  code_challenge_methods_supported:\n  - S256\n  probe:\n    url: https://api.mavenlink.com/mcp\n\
  \    method: POST tools/list\n    http_status: 401\n    www_authenticate: >-\n      Bearer realm=\"Doorkeeper\", error=\"invalid_token\",\n      resource_metadata=\"https://api.mavenlink.com/.well-known/oauth-protected-resource\"\n    checked: '2026-08-25'\ngaps:\n- >-\n  The published Swagger 2.0 contract defines two securityDefinitions but applies neither: there is no global\n  `security` block and none of the 419 operations carries an operation-level `security` array. A generated client\n  reading only the spec would not send an Authorization header, even though every endpoint requires one.\n- >-\n  The oauth2 securityDefinition declares an empty `scopes` map, so the scope names published in the discovery\n  documents (api_only, openid, email, profile, mcp, offline_access) are invisible to spec-driven tooling.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mavenlink/refs/heads/main/authentication/mavenlink-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Professional Services Automation
- Project Management
- Resource Management
- Time Tracking
- Expense Management
- Invoicing
- Project Accounting
- Business Intelligence
- Workflow Automation
- MCP
- agent-native
- Company
---
