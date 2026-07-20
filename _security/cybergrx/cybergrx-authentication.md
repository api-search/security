---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cybergrx Authentication
name_suffix: Authentication
oauth_flows: []
overview: CyberGRX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CyberGRX
provider_slug: cybergrx
scheme_count: 1
schemes:
- description: Account-generated API token sent verbatim in the Authorization header (not a Bearer prefix in the published examples). Provisioned in the GRX user-management UI; Demo/Production credentials are provisioned by a GRX representative.
  in: header
  name: ApiToken
  parameter_name: Authorization
  sources:
  - https://github.com/CyberGRX/api-examples/blob/master/HOW-TO.md
  - https://github.com/CyberGRX/api-examples/blob/master/python_examples/order_assessments/order.py
  type: apiKey
slug: cybergrx-authentication
source_filename: cybergrx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/CyberGRX/api-examples/blob/master/HOW-TO.md\ndocs: https://api.cybergrx.com/v1/swagger/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  The CyberGRX / ProcessUnity Global Risk Exchange (GRX) API authenticates with\n  a long-lived API token passed in the HTTP `Authorization` request header on\n  every call. Tokens are self-service: an account admin creates one under\n  \"Manage my company user accounts\" -> \"Access Tokens\" -> \"Add a new token\", and\n  the secret is shown only once at creation. The same token authorizes the v1,\n  bulk-v1, and v2 namespaces and the Swagger \"Authorize\" dialog. There is no\n  OAuth2/OIDC flow documented on the public surface.\nschemes:\n  - name: ApiToken\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    description: >-\n      Account-generated API token sent verbatim in the Authorization header\n      (not\
  \ a Bearer prefix in the published examples). Provisioned in the GRX\n      user-management UI; Demo/Production credentials are provisioned by a GRX\n      representative.\n    sources:\n      - https://github.com/CyberGRX/api-examples/blob/master/HOW-TO.md\n      - https://github.com/CyberGRX/api-examples/blob/master/python_examples/order_assessments/order.py\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybergrx/refs/heads/main/authentication/cybergrx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Third Party Risk
- Vendor Risk Management
- Risk Management
- GRC
- Security Assessment
---
