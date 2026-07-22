---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Simpliroute Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simpliroute secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simpliroute
provider_slug: simpliroute
scheme_count: 1
schemes:
- description: 'All SimpliRoute API requests authenticate with a static API token passed in the Authorization header as "Authorization: Token <your_token>". The token is issued per account and retrieved from the user profile in the SimpliRoute web app.'
  in: header
  name: TokenAuth
  parameter_name: Authorization
  sources:
  - https://documentation.simpliroute.com/#authentication
  token_source: https://app2.simpliroute.com/#/uprofile/info
  type: apiKey
  value_prefix: 'Token '
  verify_operation: GET https://api.simpliroute.com/v1/accounts/me/
slug: simpliroute-authentication
source_filename: simpliroute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://documentation.simpliroute.com/#authentication\ndocs: https://documentation.simpliroute.com/#authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: TokenAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    value_prefix: \"Token \"\n    description: >-\n      All SimpliRoute API requests authenticate with a static API token passed in the\n      Authorization header as \"Authorization: Token <your_token>\". The token is issued\n      per account and retrieved from the user profile in the SimpliRoute web app.\n    token_source: https://app2.simpliroute.com/#/uprofile/info\n    verify_operation: \"GET https://api.simpliroute.com/v1/accounts/me/\"\n    sources: [https://documentation.simpliroute.com/#authentication]\nnotes:\n  - HTTP Token authentication (Django REST Framework style); no OAuth2 / OIDC surface is documented.\n  - CORS is supported;\
  \ the docs warn never to expose the token in client-side code.\n  - A 14-day free trial account (https://app2.simpliroute.com/#/signup) issues a working token for testing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpliroute/refs/heads/main/authentication/simpliroute-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Route Optimization
- Last Mile Delivery
- Delivery Management
- Fleet Management
- Transportation
- Webhooks
---
