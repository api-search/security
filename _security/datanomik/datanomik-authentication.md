---
api_key_in: []
api_specs:
- filename: datanomik-accounts-api-openapi.yml
  format: yaml
  label: Datanomik Accounts API
  slug: datanomik-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-accounts-api-openapi.yml
- filename: datanomik-applications-api-openapi.yml
  format: yaml
  label: Datanomik Applications API
  slug: datanomik-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-applications-api-openapi.yml
- filename: datanomik-balances-api-openapi.yml
  format: yaml
  label: Datanomik Balances API
  slug: datanomik-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-balances-api-openapi.yml
- filename: datanomik-general-owners-api-openapi.yml
  format: yaml
  label: Datanomik General Owners API
  slug: datanomik-general-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-general-owners-api-openapi.yml
- filename: datanomik-investments-api-openapi.yml
  format: yaml
  label: Datanomik Investments API
  slug: datanomik-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-investments-api-openapi.yml
- filename: datanomik-links-api-openapi.yml
  format: yaml
  label: Datanomik Links API
  slug: datanomik-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-links-api-openapi.yml
- filename: datanomik-payment-slips-api-openapi.yml
  format: yaml
  label: Datanomik Payment Slips API
  slug: datanomik-payment-slips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-payment-slips-api-openapi.yml
- filename: datanomik-payments-api-openapi.yml
  format: yaml
  label: Datanomik Payments API
  slug: datanomik-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-payments-api-openapi.yml
- filename: datanomik-pix-transactions-api-openapi.yml
  format: yaml
  label: Datanomik Pix Transactions API
  slug: datanomik-pix-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-pix-transactions-api-openapi.yml
- filename: datanomik-transactions-api-openapi.yml
  format: yaml
  label: Datanomik Transactions API
  slug: datanomik-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-transactions-api-openapi.yml
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
