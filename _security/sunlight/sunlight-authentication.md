---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sunlight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunlight secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sunlight
provider_slug: sunlight
scheme_count: 1
schemes:
- description: 'Bearer-token authentication. The API key is issued by Sunlight support and passed as a Bearer token in the Authorization header, e.g. "Authorization: Bearer <api_key>". Keys are long-lived secrets and carry account privileges; the docs warn not to expose them in client-side code or public repositories.'
  in: header
  name: bearerAuth
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://docs.sunlight.is/
  type: http
slug: sunlight-authentication
source_filename: sunlight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sunlight.is/ (Authentication section)\ndocs: https://docs.sunlight.is/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer-token authentication. The API key is issued by Sunlight support and\n    passed as a Bearer token in the Authorization header, e.g.\n    \"Authorization: Bearer <api_key>\". Keys are long-lived secrets and carry\n    account privileges; the docs warn not to expose them in client-side code or\n    public repositories.\n  in: header\n  parameter_name: Authorization\n  sources:\n  - https://docs.sunlight.is/\nnotes: >-\n  Sunlight uses a single opaque Bearer API key per account (no OAuth2, no OIDC,\n  no per-scope tokens). There is no self-service key issuance documented — keys\n  are provisioned by Sunlight support (\"Sign Up for a Developer Key\"). Because\n  the model is a single bearer\
  \ secret, there is no OAuth scopes artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunlight/refs/heads/main/authentication/sunlight-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Education
- EdTech
- Learning
- Budgeting
- Spending
- Fintech
- JSON:API
- Groups
- Orders
---
