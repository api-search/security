---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fidor Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fidor Bank secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fidor Bank
provider_slug: fidor-bank
scheme_count: 1
schemes:
- description: OAuth2 authorization-code flow. The official Ruby client exposes authorize_start / authorize_complete helpers to obtain an access token that is then used as a bearer token against the classic transfer, account and transaction APIs.
  environments:
  - host_pattern: '*.sandbox.fidor.com'
    name: sandbox
  - host_pattern: '*.fidor.de'
    name: production
  flow: authorizationCode
  name: OAuth2
  sources:
  - https://github.com/fidor/fidor_api
  token_type: bearer
  type: oauth2
slug: fidor-bank-authentication
source_filename: fidor-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/fidor/fidor_api\ndocs: https://github.com/fidor/fidor_api#readme\nnotes: >-\n  No OpenAPI/Swagger spec is retrievable (the Stoplight-hosted docs at\n  api-docs.fidor.de and api-docs.sandbox.fidor.com are offline and fidor.com is a\n  parked domain), so this profile is searched from the official Ruby client's\n  documentation rather than derived from a spec. The Fidor REST API used OAuth2\n  with the authorization-code flow; bearer access tokens were then presented to\n  the API.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    token_type: bearer\n    environments:\n      - name: sandbox\n        host_pattern: '*.sandbox.fidor.com'\n      - name: production\n        host_pattern: '*.fidor.de'\n    sources: [https://github.com/fidor/fidor_api]\n    description: >-\n      OAuth2 authorization-code flow. The official\
  \ Ruby client exposes\n      authorize_start / authorize_complete helpers to obtain an access token\n      that is then used as a bearer token against the classic transfer, account\n      and transaction APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fidor-bank/refs/heads/main/authentication/fidor-bank-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Open Banking
- Digital Bank
- Neobank
- Germany
- Retired
---
