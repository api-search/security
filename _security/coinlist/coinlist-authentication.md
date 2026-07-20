---
api_key_in: []
api_specs:
- filename: coinlist-passage-openapi-original.json
  format: json
  label: CoinList Passage (Frontline API)
  slug: coinlist-passage-frontline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-passage-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Coinlist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: CoinList secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: CoinList
provider_slug: coinlist
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization and token endpoints
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/coinlist-passage-openapi-original.json
  type: oauth2
- description: Session token for user authentication during OAuth authorization
  name: TokenAuth
  scheme: bearer
  sources:
  - openapi/coinlist-passage-openapi-original.json
  type: http
slug: coinlist-authentication
source_filename: coinlist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coinlist-passage-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 0\n  description: OAuth 2.0 authorization and token endpoints\n  sources:\n  - openapi/coinlist-passage-openapi-original.json\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  description: Session token for user authentication during OAuth authorization\n  sources:\n  - openapi/coinlist-passage-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/authentication/coinlist-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fintech
- Cryptocurrency
- Token Sales
- Tokenized Equities
- KYC
- OAuth
- Blockchain
- Digital Assets
- Embedded Finance
---
