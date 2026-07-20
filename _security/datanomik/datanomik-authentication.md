---
api_key_in: []
api_specs:
- filename: datanomik-openbanking-openapi.json
  format: json
  label: Datanomik OpenBanking API
  slug: datanomik-openbanking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-openbanking-openapi.json
- filename: datanomik-remuneration-openapi.json
  format: json
  label: Datanomik Treasury / Remuneration API
  slug: datanomik-treasury-remuneration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-remuneration-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Datanomik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datanomik secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datanomik
provider_slug: datanomik
scheme_count: 1
schemes:
- description: HTTP Basic auth using generated API keys (secretId / secretPassword).
  name: sec0
  scheme: basic
  sources:
  - openapi/datanomik-openbanking-openapi.json
  - openapi/datanomik-remuneration-openapi.json
  type: http
slug: datanomik-authentication
source_filename: datanomik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/datanomik-openbanking-openapi.json, openapi/datanomik-remuneration-openapi.json\ndocs: https://docs.datanomik.com/docs/create-account\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  model: api-keys-http-basic\nnotes: >-\n  Datanomik authenticates every request with HTTP Basic credentials. After creating a\n  dashboard account you generate a pair of API keys - secretId (username) and\n  secretPassword (password) - at https://dashboard.datanomik.com/#/settings/api-keys and\n  send them as HTTP Basic auth. The secretPassword is shown only once at generation time\n  and cannot be recovered; if lost you must regenerate the key pair. Keys are scoped per\n  environment (sandbox vs production) and links created in one environment cannot be used\n  in another. Role-based access (e.g. ROLE_PAYMENTS_READ, ROLE_INVESTMENTS_READ) governs\n  which endpoints a key pair can call.\nschemes:\n- name: sec0\n  type: http\n\
  \  scheme: basic\n  description: HTTP Basic auth using generated API keys (secretId / secretPassword).\n  sources:\n  - openapi/datanomik-openbanking-openapi.json\n  - openapi/datanomik-remuneration-openapi.json\nroles:\n- ROLE_PAYMENTS_READ\n- ROLE_INVESTMENTS_READ\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/authentication/datanomik-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Open Finance
- Open Banking
- Treasury Management
- Cash Management
- Payments
- PIX
- Financial Data
- Bank Connectivity
- Brazil
- LatAm
- Fintech
---
