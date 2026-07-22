---
api_key_in: []
api_specs:
- filename: trueaccord-recover-openapi.yml
  format: yaml
  label: TrueAccord Recover API
  slug: trueaccord-recover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueaccord/refs/heads/main/openapi/trueaccord-recover-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Trueaccord Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueAccord secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueAccord
provider_slug: trueaccord
scheme_count: 1
schemes:
- description: 'API key as HTTP Basic username (password ignored, trailing colon required). Example: curl https://api.trueaccord.com/api/v1/customers/ -u $YOUR_KEY:'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/trueaccord-recover-openapi.yml
  type: http
slug: trueaccord-authentication
source_filename: trueaccord-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.trueaccord.com/recover/recover-api-reference\ndocs: https://docs.trueaccord.com/recover/recover-api-reference\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    HTTP Basic authentication over HTTPS. The TrueAccord API key is supplied as\n    the username; the password field is ignored but a trailing colon is\n    required. Multi-creditor accounts must also send the X-TA-CREDITOR header\n    identifying the creditor, or the API returns 403.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      API key as HTTP Basic username (password ignored, trailing colon\n      required). Example: curl https://api.trueaccord.com/api/v1/customers/ -u $YOUR_KEY:\n    sources: [openapi/trueaccord-recover-openapi.yml]\nadditional_headers:\n  - name: X-TA-CREDITOR\n    required_when: multi-creditor account\n    description: Creditor id;\
  \ required for multi-creditor accounts, else 403.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trueaccord/refs/heads/main/authentication/trueaccord-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Debt Collection
- Financial Services
- Fintech
- Machine Learning
- Collections
- Consumer Finance
---
