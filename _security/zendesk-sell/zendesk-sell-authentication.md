---
api_key_in: []
api_specs:
- filename: zendesk-sell.postman_collection.json
  format: json
  label: Zendesk Sell (Sales CRM) API
  slug: sales-crm-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/collections/zendesk-sell.postman_collection.json
- filename: zendesk-sell-contacts-api-openapi.yml
  format: yaml
  label: Zendesk Sell Contacts API
  slug: zendesk-sell-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-contacts-api-openapi.yml
- filename: zendesk-sell-deals-api-openapi.yml
  format: yaml
  label: Zendesk Sell Deals API
  slug: zendesk-sell-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-deals-api-openapi.yml
- filename: zendesk-sell-leads-api-openapi.yml
  format: yaml
  label: Zendesk Sell Leads API
  slug: zendesk-sell-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-leads-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zendesk Sell Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- refreshToken
overview: Zendesk Sell secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and refreshToken flow(s).
provider_name: Zendesk Sell
provider_slug: zendesk-sell
scheme_count: 1
schemes:
- description: OAuth 2.0 with four documented grants — authorization code (web apps), implicit (user-agent/desktop/mobile), resource owner password credentials, and refresh token.
  flows:
  - authorizationUrl: https://api.getbase.com/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.getbase.com/oauth2/token
  - authorizationUrl: https://api.getbase.com/oauth2/authorize
    flow: implicit
    scopes: 3
  - flow: password
    scopes: 3
    tokenUrl: https://api.getbase.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://api.getbase.com/oauth2/token
  name: oauth2
  sources:
  - openapi/_original/zendesk-sell-openapi.yml
  - https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/
  type: oauth2
slug: zendesk-sell-authentication
source_filename: zendesk-sell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/zendesk-sell-openapi.yml\ndocs: https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\nreference: https://developer.zendesk.com/api-reference/sales-crm/authentication/reference/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - password\n  - refreshToken\n  bearer_header: 'Authorization: Bearer <access_token>'\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getbase.com/oauth2/authorize\n    tokenUrl: https://api.getbase.com/oauth2/token\n    scopes: 3\n  - flow: implicit\n    authorizationUrl: https://api.getbase.com/oauth2/authorize\n    scopes: 3\n  - flow: password\n    tokenUrl: https://api.getbase.com/oauth2/token\n    scopes: 3\n  - flow: refreshToken\n    tokenUrl: https://api.getbase.com/oauth2/token\n  description: >-\n    OAuth 2.0 with four documented grants —\
  \ authorization code (web apps), implicit\n    (user-agent/desktop/mobile), resource owner password credentials, and refresh token.\n  sources:\n  - openapi/_original/zendesk-sell-openapi.yml\n  - https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\nendpoints:\n- path: /oauth2/authorize\n  purpose: Authorization endpoint\n- path: /oauth2/token\n  purpose: Token endpoint (also used by the refresh-token grant)\n- path: /oauth2/revoke\n  purpose: Token revocation\n- path: /oauth2/token/info\n  purpose: Token introspection / validation\ntoken_model:\n  single_user:\n    mechanism: dashboard-generated personal access token\n    lifetime: unlimited\n    note: >-\n      Sell administrators can mint access tokens from the Sell dashboard that never expire —\n      these behave like API keys and are the documented path for single-user integrations.\n  multi_user:\n    mechanism: OAuth 2.0 authorization on behalf of the resource owner\n    access_token_lifetime: 1 hour\n\
  \    refresh_token_lifetime: no expiration\n    note: >-\n      The preferred integration model; access tokens obtained from the token endpoint expire\n      after one hour and are renewed with the refresh token.\noidc: false\nmtls: false\nnotes:\n- >-\n  api.getbase.com serves no /.well-known/oauth-authorization-server and no\n  /.well-known/openid-configuration (both 404 on 2026-08-13), so the OAuth metadata must be\n  read from the human docs — there is no RFC 8414 discovery document.\n- >-\n  The same Zendesk access token is reusable across Zendesk APIs for the Sync API.\nx-evidence:\n- url: https://developer.zendesk.com/api-reference/sales-crm/authentication/introduction/\n  status: 200\n- url: https://developer.zendesk.com/api-reference/sales-crm/authentication/reference/\n  status: 200\n- url: https://api.getbase.com/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/authentication/zendesk-sell-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Sales
- Sales Automation
- Leads
- Deals
- Pipeline
- Customer Experience
---
