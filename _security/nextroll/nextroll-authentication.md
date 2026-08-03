---
api_key_in:
- query
auth_types:
- oauth2
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nextroll Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- refreshToken
overview: NextRoll secures its APIs with oauth2, apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and refreshToken flow(s).
provider_name: NextRoll
provider_slug: nextroll
scheme_count: 5
schemes:
- applies_to: every NextRoll API request on services.adroll.com
  description: The consumer key of an application registered at developers.nextroll.com. Always sent in the URL query string regardless of HTTP method — it must not be placed in a POST/PUT/PATCH body. Registration and an API key have been mandatory since the move from api.adroll.com / app.adroll.com to services.adroll.com.
  in: query
  name: application_api_key
  obtain: https://developers.nextroll.com/my-apps/new-app
  parameter: apikey
  required: true
  type: apiKey
- description: Personal Access Token identifying the AdRoll user, paired with the application `apikey` query parameter which identifies the calling application. Intended for simple integrations and scripts; the docs direct multi-user applications to OAuth instead.
  format: 'Authorization: Token MYTOKEN'
  header: Authorization
  in: header
  manage: https://app.adroll.com/settings/personal-access-tokens
  name: personal_access_token
  scheme: Token
  type: http
- authorizationUrl: https://services.adroll.com/auth/authorize
  bearer_transport:
  - Authorization header, Bearer scheme
  - access_token form-encoded body parameter
  - access_token URL query parameter
  conforms:
  - RFC 6749
  - RFC 6750
  flows:
  - flow: authorizationCode
    note: three-legged; the most commonly used grant
  - flow: implicit
    note: for clients that cannot keep a secret, e.g. single-page apps
  - flow: password
    note: Resource Owner Password Credentials — documented as a last resort
  - flow: refreshToken
  name: oauth2
  scope_note: A single coarse scope today. The docs state fine-grained scopes are planned but not implemented.
  scopes:
  - description: Access to all resources; the default when no scope is specified.
    scope: all
  tokenUrl: https://services.adroll.com/auth/token
  token_lifetime:
    access_token: 24 hours, all grant types
    refresh_token: one year, and single-use — a new refresh token is issued with every new access token
  type: oauth2
- applies_to: NextRoll Server-to-Server (S2S) Event API on srv.adroll.com
  description: Server Access Tokens (SATs) are required for the S2S event endpoint. They are not self-service — an account manager issues them and shares them out of band via a one-time, seven-day 1Password share link.
  docs: https://apidocs.nextroll.com/server-to-server-api/reference.html
  name: server_access_token
  obtain: contact your NextRoll account manager
  type: apiKey
- applies_to: AdRoll MCP Server at https://services.adroll.com/mcp
  authorizationUrl: https://services.adroll.com/mcp/auth/authorize
  code_challenge_methods:
  - S256
  conforms:
  - RFC 8414
  - RFC 9728
  - OAuth 2.1 / PKCE
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  introspectionUrl: https://services.adroll.com/mcp/auth/introspect
  issuer: https://services.adroll.com/mcp
  name: mcp_oauth21
  registrationUrl: https://services.adroll.com/mcp/auth/register
  revocationUrl: https://services.adroll.com/mcp/auth/revoke
  scopes:
  - description: The single scope advertised by the MCP authorization server.
    scope: mcp
  source: well-known/nextroll-oauth-authorization-server.json
  tokenUrl: https://services.adroll.com/mcp/auth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: nextroll-authentication
source_filename: nextroll-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://apidocs.nextroll.com/guides/get-started.html\ndocs:\n- https://apidocs.nextroll.com/guides/get-started.html\n- https://apidocs.nextroll.com/guides/oauth.html\n- https://apidocs.nextroll.com/guides/api-key-migration.html\n- https://services.adroll.com/.well-known/oauth-authorization-server\nderived_from_openapi: false\nderived_from_openapi_note: NextRoll publishes no OpenAPI document, so this profile is\n  read from the published authentication guides and the RFC 8414 metadata rather than\n  from securitySchemes.\nsummary:\n  types: [oauth2, apiKey, http, oauth2]\n  api_key_in: [query]\n  api_key_names: [apikey]\n  http_schemes: [bearer, token]\n  oauth2_flows: [authorizationCode, implicit, password, refreshToken]\n  every_request_requires_api_key: true\nschemes:\n- name: application_api_key\n  type: apiKey\n  in: query\n  parameter: apikey\n  required: true\n  applies_to: every NextRoll API request on services.adroll.com\n\
  \  description: >-\n    The consumer key of an application registered at developers.nextroll.com. Always\n    sent in the URL query string regardless of HTTP method — it must not be placed in\n    a POST/PUT/PATCH body. Registration and an API key have been mandatory since the\n    move from api.adroll.com / app.adroll.com to services.adroll.com.\n  obtain: https://developers.nextroll.com/my-apps/new-app\n- name: personal_access_token\n  type: http\n  scheme: Token\n  in: header\n  header: Authorization\n  format: 'Authorization: Token MYTOKEN'\n  description: >-\n    Personal Access Token identifying the AdRoll user, paired with the application\n    `apikey` query parameter which identifies the calling application. Intended for\n    simple integrations and scripts; the docs direct multi-user applications to OAuth\n    instead.\n  manage: https://app.adroll.com/settings/personal-access-tokens\n- name: oauth2\n  type: oauth2\n  conforms:\n  - RFC 6749\n  - RFC 6750\n  authorizationUrl:\
  \ https://services.adroll.com/auth/authorize\n  tokenUrl: https://services.adroll.com/auth/token\n  flows:\n  - flow: authorizationCode\n    note: three-legged; the most commonly used grant\n  - flow: implicit\n    note: for clients that cannot keep a secret, e.g. single-page apps\n  - flow: password\n    note: Resource Owner Password Credentials — documented as a last resort\n  - flow: refreshToken\n  token_lifetime:\n    access_token: 24 hours, all grant types\n    refresh_token: one year, and single-use — a new refresh token is issued with every\n      new access token\n  bearer_transport:\n  - Authorization header, Bearer scheme\n  - access_token form-encoded body parameter\n  - access_token URL query parameter\n  scopes:\n  - scope: all\n    description: Access to all resources; the default when no scope is specified.\n  scope_note: >-\n    A single coarse scope today. The docs state fine-grained scopes are planned but\n    not implemented.\n- name: server_access_token\n  type: apiKey\n\
  \  applies_to: NextRoll Server-to-Server (S2S) Event API on srv.adroll.com\n  description: >-\n    Server Access Tokens (SATs) are required for the S2S event endpoint. They are not\n    self-service — an account manager issues them and shares them out of band via a\n    one-time, seven-day 1Password share link.\n  obtain: contact your NextRoll account manager\n  docs: https://apidocs.nextroll.com/server-to-server-api/reference.html\n- name: mcp_oauth21\n  type: oauth2\n  applies_to: AdRoll MCP Server at https://services.adroll.com/mcp\n  conforms:\n  - RFC 8414\n  - RFC 9728\n  - OAuth 2.1 / PKCE\n  issuer: https://services.adroll.com/mcp\n  authorizationUrl: https://services.adroll.com/mcp/auth/authorize\n  tokenUrl: https://services.adroll.com/mcp/auth/token\n  registrationUrl: https://services.adroll.com/mcp/auth/register\n  revocationUrl: https://services.adroll.com/mcp/auth/revoke\n  introspectionUrl: https://services.adroll.com/mcp/auth/introspect\n  dynamic_client_registration:\
  \ true\n  code_challenge_methods: [S256]\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  scopes:\n  - scope: mcp\n    description: The single scope advertised by the MCP authorization server.\n  source: well-known/nextroll-oauth-authorization-server.json\nobservations:\n- >-\n  Two distinct OAuth deployments coexist: the legacy RFC 6749 developer OAuth on\n  /auth/* with a single `all` scope, and a modern OAuth 2.1 + DCR + PKCE deployment on\n  /mcp/auth/* with an `mcp` scope. The MCP path is materially more current than the API\n  path.\n- The developer OAuth still advertises the implicit and resource-owner-password\n  grants, both of which OAuth 2.1 removes.\n- The `apikey` credential is transmitted in the URL query string on every call, and\n  the OAuth guide also permits `access_token` in the query string — both leak into\n  logs, proxies and referrers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextroll/refs/heads/main/authentication/nextroll-authentication.yml
summary_line: oauth2/apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Advertising
- AdTech
- Marketing
- Account Based Marketing
- Retargeting
- Audiences
- Campaign Management
- Analytics
- Reporting
- MarTech
- Agents
---
