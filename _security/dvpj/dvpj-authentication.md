---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dvpj Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Conta Azul secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Conta Azul
provider_slug: dvpj
scheme_count: 2
schemes:
- authorizationUrl: https://auth.contaazul.com/login
  client_authentication: basic
  flow: authorizationCode
  name: OAuth2
  scopes:
  - openid
  - profile
  - aws.cognito.signin.user.admin
  sources:
  - https://developers.contaazul.com/auth
  tokenUrl: https://auth.contaazul.com/oauth2/token
  type: oauth2
- bearerFormat: JWT
  description: Bearer JWT access_token sent on every API request
  name: BearerAuth
  scheme: bearer
  sources:
  - https://developers.contaazul.com/makingcalls
  - https://developers.contaazul.com/docs/financial-apis-openapi
  type: http
slug: dvpj-authentication
source_filename: dvpj-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.contaazul.com/auth\ndocs: https://developers.contaazul.com/auth\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  client_authentication: basic\n  bearer_format: JWT\nnotes: >-\n  Conta Azul API authenticates with OAuth 2.0 Authorization Code flow backed by\n  AWS Cognito. The client exchanges the authorization code for tokens at the\n  token endpoint using HTTP Basic auth (Base64 of client_id:client_secret).\n  API calls carry the access_token as a Bearer JWT in the Authorization header.\n  access_token TTL is 3600s (1h); refresh_token is valid up to 5 years or until\n  the next renewal (a new refresh_token is returned on every renewal).\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://auth.contaazul.com/login\n    tokenUrl: https://auth.contaazul.com/oauth2/token\n    client_authentication: basic\n    scopes:\n      - openid\n  \
  \    - profile\n      - aws.cognito.signin.user.admin\n    sources: [https://developers.contaazul.com/auth]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer JWT access_token sent on every API request\n    sources: [https://developers.contaazul.com/makingcalls, https://developers.contaazul.com/docs/financial-apis-openapi]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dvpj/refs/heads/main/authentication/dvpj-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- ERP
- Financial
- Accounting
- Invoicing
- Payments
- SMB
- Brazil
- OAuth
---
