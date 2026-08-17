---
api_key_in: []
api_specs:
- filename: unbounce-accounts-api-openapi.yml
  format: yaml
  label: Unbounce Accounts API
  slug: unbounce-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-accounts-api-openapi.yml
- filename: unbounce-domains-api-openapi.yml
  format: yaml
  label: Unbounce Domains API
  slug: unbounce-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-domains-api-openapi.yml
- filename: unbounce-leads-api-openapi.yml
  format: yaml
  label: Unbounce Leads API
  slug: unbounce-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-leads-api-openapi.yml
- filename: unbounce-meta-api-openapi.yml
  format: yaml
  label: Unbounce Meta API
  slug: unbounce-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-meta-api-openapi.yml
- filename: unbounce-pagegroups-api-openapi.yml
  format: yaml
  label: Unbounce PageGroups API
  slug: unbounce-pagegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-pagegroups-api-openapi.yml
- filename: unbounce-pages-api-openapi.yml
  format: yaml
  label: Unbounce Pages API
  slug: unbounce-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-pages-api-openapi.yml
- filename: unbounce-users-api-openapi.yml
  format: yaml
  label: Unbounce Users API
  slug: unbounce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Unbounce Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Unbounce secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Unbounce
provider_slug: unbounce
scheme_count: 3
schemes:
- availability: All pricing plans, after an approved API Access request
  credential: Unbounce API key as the username, empty password
  errors:
  - meaning: API key missing
    status: 401
  - meaning: API key forbidden to access the resource
    status: 403
  example: 'curl -u API_KEY: -H "Accept: application/vnd.unbounce.api.v0.4+json" https://api.unbounce.com/accounts'
  location: Authorization header (HTTP Basic)
  name: api_key
  permissions: Unscoped. "API keys currently act like Unbounce account administrators" — read access to Accounts, Sub Accounts/Clients, Domains, Page Groups, Pages, Leads and Users.
  provisioning: Not self-serve. Submit the API Access form, wait for Unbounce support to enable access ("a couple of days"), then create keys in the app under Manage Account -> API Access.
  rotation: Multiple keys can be created per account; no documented expiry or rotation policy.
  scheme: basic
  sources:
  - raml/unbounce-api-v0.4.raml
  - https://developer.unbounce.com/getting_started/#Authorization
  surface: REST API v0.4
  type: http
- errors:
  - meaning: access token missing
    status: 401
  - meaning: bad or expired access token
    status: 403
  expires_in: 600
  flows:
  - authorizationUrl: https://api.unbounce.com/oauth/authorize
    flow: authorizationCode
    refreshTokenUrl: https://api.unbounce.com/oauth/token
    scope_names:
    - full
    scopes: 1
    tokenUrl: https://api.unbounce.com/oauth/token
  location: 'Authorization: Bearer <token>'
  name: oauth2
  note: The RAML securityScheme settings name developer.unbounce.com for both OAuth URIs, while the prose docs and every worked example name api.unbounce.com. api.unbounce.com is the one to use; the RAML's baseUri is likewise developer.unbounce.com where the live API is api.unbounce.com — a known inconsistency in Unbounce's published spec.
  permissions: OAuth tokens grant exactly the permissions the authenticating user already has.
  provisioning: Not self-serve. "We''re still working on providing self-service for OAuth applications" — client credentials are granted case-by-case via a registration form.
  refresh: grant_type=refresh_token; a new refresh token is issued on each exchange
  sources:
  - raml/unbounce-api-v0.4.raml
  - https://developer.unbounce.com/getting_started/#Authorization
  surface: REST API v0.4
  token_format: JWT
  token_type: bearer
  type: oauth2
- challenge: 'WWW-Authenticate: Bearer resource_metadata="https://mcp.unbounce.com/.well-known/oauth-protected-resource", scope="unbounce"'
  client_id_metadata_document_supported: true
  discovery:
  - path: /.well-known/oauth-authorization-server
    spec: RFC 8414
    status: 200
  - path: /.well-known/oauth-protected-resource
    spec: RFC 9728
    status: 200
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.unbounce.com/authorize
    flow: authorizationCode
    pkce: S256
    scope_names:
    - unbounce
    scopes: 1
    tokenUrl: https://mcp.unbounce.com/token
  issuer: https://mcp.unbounce.com
  name: mcp-oauth2
  provisioning: Fully self-serve and machine-negotiable — the opposite of the REST surface. A client registers dynamically and the user consents on Unbounce's own sign-in screen; the assistant never sees the password.
  registration_endpoint: https://mcp.unbounce.com/register
  sources:
  - https://mcp.unbounce.com/.well-known/oauth-authorization-server
  surface: MCP server (https://mcp.unbounce.com/mcp)
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: unbounce-authentication
source_filename: unbounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.unbounce.com/getting_started/#Authorization\ndocs: https://developer.unbounce.com/getting_started/#Authorization\nderived_from:\n- raml/unbounce-api-v0.4.raml\n- openapi/_original/unbounce-openapi.yml\n- well-known/unbounce-mcp-oauth-authorization-server.json\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode]\n  surfaces: [rest, mcp]\n  transport: HTTPS required\n  self_serve: false\nschemes:\n- name: api_key\n  surface: REST API v0.4\n  type: http\n  scheme: basic\n  location: Authorization header (HTTP Basic)\n  credential: Unbounce API key as the username, empty password\n  example: 'curl -u API_KEY: -H \"Accept: application/vnd.unbounce.api.v0.4+json\" https://api.unbounce.com/accounts'\n  availability: All pricing plans, after an approved API Access request\n  provisioning: >-\n    Not self-serve. Submit the API Access form, wait for Unbounce support\
  \ to enable\n    access (\"a couple of days\"), then create keys in the app under Manage Account ->\n    API Access.\n  permissions: >-\n    Unscoped. \"API keys currently act like Unbounce account administrators\" — read\n    access to Accounts, Sub Accounts/Clients, Domains, Page Groups, Pages, Leads and Users.\n  rotation: Multiple keys can be created per account; no documented expiry or rotation policy.\n  errors:\n  - {status: 401, meaning: API key missing}\n  - {status: 403, meaning: API key forbidden to access the resource}\n  sources: [raml/unbounce-api-v0.4.raml, https://developer.unbounce.com/getting_started/#Authorization]\n- name: oauth2\n  surface: REST API v0.4\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.unbounce.com/oauth/authorize\n    tokenUrl: https://api.unbounce.com/oauth/token\n    refreshTokenUrl: https://api.unbounce.com/oauth/token\n    scopes: 1\n    scope_names: [full]\n  token_format: JWT\n  token_type: bearer\n \
  \ expires_in: 600\n  refresh: 'grant_type=refresh_token; a new refresh token is issued on each exchange'\n  location: 'Authorization: Bearer <token>'\n  provisioning: >-\n    Not self-serve. \"We''re still working on providing self-service for OAuth\n    applications\" — client credentials are granted case-by-case via a registration form.\n  permissions: OAuth tokens grant exactly the permissions the authenticating user already has.\n  errors:\n  - {status: 401, meaning: access token missing}\n  - {status: 403, meaning: bad or expired access token}\n  sources: [raml/unbounce-api-v0.4.raml, https://developer.unbounce.com/getting_started/#Authorization]\n  note: >-\n    The RAML securityScheme settings name developer.unbounce.com for both OAuth URIs,\n    while the prose docs and every worked example name api.unbounce.com. api.unbounce.com\n    is the one to use; the RAML's baseUri is likewise developer.unbounce.com where the\n    live API is api.unbounce.com — a known inconsistency in Unbounce's\
  \ published spec.\n- name: mcp-oauth2\n  surface: MCP server (https://mcp.unbounce.com/mcp)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.unbounce.com/authorize\n    tokenUrl: https://mcp.unbounce.com/token\n    pkce: S256\n    scopes: 1\n    scope_names: [unbounce]\n  issuer: https://mcp.unbounce.com\n  registration_endpoint: https://mcp.unbounce.com/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  discovery:\n  - {path: /.well-known/oauth-authorization-server, spec: RFC 8414, status: 200}\n  - {path: /.well-known/oauth-protected-resource, spec: RFC 9728, status: 200}\n  challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.unbounce.com/.well-known/oauth-protected-resource\", scope=\"unbounce\"'\n  provisioning: >-\n    Fully self-serve and machine-negotiable — the opposite of the REST surface. A client\n    registers dynamically and\
  \ the user consents on Unbounce's own sign-in screen; the\n    assistant never sees the password.\n  sources: [https://mcp.unbounce.com/.well-known/oauth-authorization-server]\nobservation: >-\n  Unbounce's two authentication surfaces are a generation apart. The REST API requires a\n  human support ticket for a key and a case-by-case grant for an OAuth client, with one\n  unscoped all-or-nothing permission level. The MCP server implements the modern\n  authorization stack — RFC 8414 metadata, RFC 9728 protected-resource metadata, PKCE and\n  RFC 7591 dynamic registration — and can be authorized by an agent with no human in the\n  loop beyond consent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/authentication/unbounce-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Landing Pages
- Conversion Rate Optimization
- Marketing
- A/B Testing
- Lead Generation
- Marketing Automation
---
