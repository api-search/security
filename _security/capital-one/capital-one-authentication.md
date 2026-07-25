---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Capital One Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Capital One secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Capital One
provider_slug: capital-one
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    note: 'Client credentials grant. Partners obtain a client_id / client_secret via the DevExchange program and exchange them for a short-lived bearer token presented on each API call as `Authorization: Bearer <token>`.'
    sandbox_tokenUrl: https://api-sandbox.capitalone.com/oauth2/token
    tokenUrl: https://api.capitalone.com/oauth2/token
  name: OAuth2
  sources:
  - https://developer.capitalone.com/documentation/o-auth
  type: oauth2
slug: capital-one-authentication
source_filename: capital-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.capitalone.com/documentation/o-auth\ndocs: https://developer.capitalone.com/documentation/o-auth\nnotes: >-\n  Capital One does not publish a downloadable OpenAPI, so this profile is\n  captured from the DevExchange OAuth documentation rather than derived from\n  securitySchemes. All DevExchange partner APIs are secured with OAuth 2.0.\n  Access to production is gated behind partner approval; the sandbox\n  (api-sandbox.capitalone.com) is used for pre-production integration.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  transport: header\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.capitalone.com/oauth2/token\n    sandbox_tokenUrl: https://api-sandbox.capitalone.com/oauth2/token\n    note: >-\n      Client credentials grant. Partners obtain a client_id / client_secret via\n      the DevExchange program\
  \ and exchange them for a short-lived bearer token\n      presented on each API call as `Authorization: Bearer <token>`.\n  sources: [https://developer.capitalone.com/documentation/o-auth]\nrelated:\n- product: Data Protection and Client Authentication Public Key Sharing API\n  role: >-\n    Supporting security primitive — clients exchange public keys with Capital\n    One to establish encrypted, authenticated communication for sensitive data\n    in transit, complementing the OAuth 2.0 bearer model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capital-one/refs/heads/main/authentication/capital-one-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Auto Finance
- Authorizations
- Banking
- Credit Cards
- Credit Offers
- DevExchange
- Financial Services
- FDX
- Open Banking
- OAuth 2.0
- Payments
- Rewards
- United States
- Fortune 500
---
