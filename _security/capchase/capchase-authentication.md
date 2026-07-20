---
api_key_in: []
api_specs:
- filename: capchase-pay-openapi.yml
  format: yaml
  label: Capchase Pay API
  slug: capchase-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capchase/refs/heads/main/openapi/capchase-pay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Capchase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capchase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capchase
provider_slug: capchase
scheme_count: 1
schemes:
- description: 'Basic auth: username=clientId, password=clientSecret. Request credentials at pay@capchase.com.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/capchase-pay-openapi.yml
  type: http
slug: capchase-authentication
source_filename: capchase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/capchase-pay-openapi.yml\ndocs: https://capchase.readme.io/reference/authentication\ncredential_request: pay@capchase.com\nnotes: >-\n  Capchase Pay uses HTTP Basic authentication. The username is the clientId and the\n  password is the clientSecret, sent as `Authorization: Basic base64(clientId:clientSecret)`.\n  Credentials are issued on request (pay@capchase.com) and the Playground environment\n  uses a separate set of keys. Unauthorized requests return 401. There is no OAuth,\n  API-key header, or scope surface.\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Basic auth: username=clientId, password=clientSecret. Request credentials at\n    pay@capchase.com.'\n  sources:\n  - openapi/capchase-pay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capchase/refs/heads/main/authentication/capchase-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- Financing
- B2B SaaS
- Revenue Financing
- BNPL
- KYB
- Underwriting
---
