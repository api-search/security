---
api_key_in:
- header
api_specs:
- filename: loopay-openapi-original.json
  format: json
  label: Loopay API
  slug: loopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-openapi-original.json
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Loopay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loopay secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loopay
provider_slug: loopay
scheme_count: 1
schemes:
- documented_only: true
  name: bearerToken
  obtained_via: POST /login (User.login)
  scheme: bearer
  sources:
  - openapi/loopay-openapi-original.json
  - https://api.loopay.com/openapi.json
  type: http
slug: loopay-authentication
source_filename: loopay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.loopay.com/openapi.json (info.description auth guide) + https://api.loopay.com/explorer\ndocs: https://api.loopay.com/explorer/#/User/User.login\nsummary:\n  types: [token]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Loopay uses a token-based authentication system. A bearer token is minted by\n    POSTing credentials to /login (operationId User.login); the token is then sent\n    on subsequent requests. The OpenAPI ships an empty components.securitySchemes\n    block, so the scheme is documented in prose (info.description) rather than\n    declared machine-readably — a gap worth filing with the provider.\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    documented_only: true\n    obtained_via: POST /login (User.login)\n    sources: [openapi/loopay-openapi-original.json, https://api.loopay.com/openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/authentication/loopay-authentication.yml
summary_line: token · 1 scheme
tags:
- Company
- Payments
- Fintech
- Banking as a Service
- Cross-Border Payments
- Payouts
- Treasury
- Latin America
---
