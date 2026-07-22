---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wrapbook Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wrapbook secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wrapbook
provider_slug: wrapbook
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.wrapbook.com/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://app.wrapbook.com/oauth/register
    revocationUrl: https://app.wrapbook.com/oauth/revoke
    scopes: 21
    tokenUrl: https://app.wrapbook.com/oauth/token
  issuer: https://app.wrapbook.com/
  name: OAuth2
  sources:
  - well-known/wrapbook-oauth-authorization-server.json
  type: oauth2
slug: wrapbook-authentication
source_filename: wrapbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.wrapbook.com/.well-known/oauth-authorization-server\nnotes: >-\n  Wrapbook publishes no public developer docs or OpenAPI, so this profile is drawn\n  from the live RFC 8414 authorization-server metadata on the production app host.\n  The server supports only the authorization-code grant with PKCE (S256), public\n  clients (token_endpoint_auth_methods_supported = none), token revocation, and\n  RFC 7591 dynamic client registration. 21 read-only scopes cover the accounting /\n  payroll / budget / purchase-order surface used by its accounting integrations.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  public_client: true\n  dynamic_client_registration: true\n  scope_count: 21\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://app.wrapbook.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.wrapbook.com/oauth/authorize\n    tokenUrl: https://app.wrapbook.com/oauth/token\n\
  \    revocationUrl: https://app.wrapbook.com/oauth/revoke\n    registrationUrl: https://app.wrapbook.com/oauth/register\n    scopes: 21\n  sources: [well-known/wrapbook-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrapbook/refs/heads/main/authentication/wrapbook-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Entertainment
- Payroll
- Production Accounting
- Accounts Payable
- Film
- Television
- Fintech
---
