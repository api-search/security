---
api_key_in: []
api_specs:
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Accept API (Singapore)
  slug: fazz-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Send API (Singapore)
  slug: fazz-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Payment Methods API
  slug: fazz-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: documented
name: Fazz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fazz secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fazz
provider_slug: fazz
scheme_count: 1
schemes:
- example: curl https://www.xfers.io/api/v4/payments -u API_KEY:SECRET_KEY
  name: basic_auth
  notes: HTTP Basic authentication. Provide your API key as the Basic auth username and your secret key as the password (base64(api_key:secret_key)) in the Authorization header. Live keys start with `live_`; sandbox keys start with `test_`. All requests must be made over HTTPS. Keys are generated on the Developer Tools page of the Fazz Business dashboard; the secret key is shown only once.
  scheme: basic
  sources:
  - https://docs.fazz.com/docs/authentication
  type: http
slug: fazz-authentication
source_filename: fazz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: documented\nsource: https://docs.fazz.com/docs/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - https://docs.fazz.com/docs/authentication\n  notes: >-\n    HTTP Basic authentication. Provide your API key as the Basic auth\n    username and your secret key as the password\n    (base64(api_key:secret_key)) in the Authorization header. Live keys\n    start with `live_`; sandbox keys start with `test_`. All requests must\n    be made over HTTPS. Keys are generated on the Developer Tools page of\n    the Fazz Business dashboard; the secret key is shown only once.\n  example: 'curl https://www.xfers.io/api/v4/payments -u API_KEY:SECRET_KEY'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/authentication/fazz-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Payments
- Business Banking
- Disbursements
- Southeast Asia
- PayNow
- Virtual Accounts
---
