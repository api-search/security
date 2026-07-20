---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hokodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hokodo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hokodo
provider_slug: hokodo
scheme_count: 1
schemes:
- description: 'Hokodo authenticates API requests with a secret API key presented in the Authorization header using the "Token" scheme (Django REST Framework TokenAuthentication). A live challenge to https://api.hokodo.co/v1/companies returns HTTP 401 with header `WWW-Authenticate: Token` and body {"detail": "Authentication credentials were not provided."}.'
  format: 'Authorization: Token <api-key>'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - probe:https://api.hokodo.co/v1/companies
  type: apiKey
slug: hokodo-authentication
source_filename: hokodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.hokodo.co/v1/companies\ndocs: https://docs.hokodo.co/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: Token\n  oauth2_flows: []\nschemes:\n  - name: TokenAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: \"Authorization: Token <api-key>\"\n    description: >-\n      Hokodo authenticates API requests with a secret API key presented in the\n      Authorization header using the \"Token\" scheme (Django REST Framework\n      TokenAuthentication). A live challenge to https://api.hokodo.co/v1/companies\n      returns HTTP 401 with header `WWW-Authenticate: Token` and body\n      {\"detail\": \"Authentication credentials were not provided.\"}.\n    sources: [probe:https://api.hokodo.co/v1/companies]\nevidence:\n  - source: https://api.hokodo.co/v1/companies\n    status: 401\n    www_authenticate: Token\n    body: '{\"detail\":\"Authentication credentials were not provided.\"\
  }'\nnotes: >-\n  Separate live and sandbox keys are issued per environment\n  (sandbox console at https://sandbox.hokodo.co). No OpenAPI specification is\n  currently published publicly, so this profile is derived from the live API\n  authentication challenge rather than a securitySchemes block.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hokodo/refs/heads/main/authentication/hokodo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- B2B Payments
- Buy Now Pay Later
- Trade Credit
- Embedded Finance
- Invoice Financing
- Payments API
---
