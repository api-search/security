---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bitwise Investments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitwise Investments secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitwise Investments
provider_slug: bitwise-investments
scheme_count: 1
schemes:
- description: API key issued by Bitwise, presented in the Authorization request header.
  in: header
  name: ApiKeyAuth
  parameter_name: Authorization
  sources:
  - https://developers.bitwiseinvestments.com/
  type: apiKey
slug: bitwise-investments-authentication
source_filename: bitwise-investments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.bitwiseinvestments.com/\ndocs: https://developers.bitwiseinvestments.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    The Bitwise API is documented via a public Postman collection. Authentication is performed with\n    an API key presented in the HTTP Authorization request header. API keys are not self-service —\n    they are issued on request by contacting api@bitwiseinvestments.com. No OpenAPI/Swagger definition\n    is published, so this profile is captured from the developer documentation rather than derived\n    from a spec.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: API key issued by Bitwise, presented in the Authorization request header.\n  sources:\n  - https://developers.bitwiseinvestments.com/\nkey_provisioning:\n  self_service: false\n  contact: api@bitwiseinvestments.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwise-investments/refs/heads/main/authentication/bitwise-investments-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Asset Management
- ETF
- Index Funds
- Market Data
- Financial Services
- Investment Management
---
