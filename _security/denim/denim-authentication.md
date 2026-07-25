---
api_key_in:
- header
api_specs:
- filename: denim-companies-api-openapi.yml
  format: yaml
  label: Denim Companies API
  slug: denim-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-companies-api-openapi.yml
- filename: denim-debtors-api-openapi.yml
  format: yaml
  label: Denim Debtors API
  slug: denim-debtors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-debtors-api-openapi.yml
- filename: denim-jobs-api-openapi.yml
  format: yaml
  label: Denim Jobs API
  slug: denim-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-jobs-api-openapi.yml
- filename: denim-jobs-v2-api-openapi.yml
  format: yaml
  label: Denim Jobs V2 API
  slug: denim-jobs-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-jobs-v2-api-openapi.yml
- filename: denim-payees-api-openapi.yml
  format: yaml
  label: Denim Payees API
  slug: denim-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-payees-api-openapi.yml
- filename: denim-transactions-api-openapi.yml
  format: yaml
  label: Denim Transactions API
  slug: denim-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Denim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Denim secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Denim
provider_slug: denim
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/denim-openapi-original.json
  type: apiKey
slug: denim-authentication
source_filename: denim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/denim-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/denim-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/authentication/denim-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Freight
- Factoring
- Payments
- Logistics
- Trucking
- Fintech
- Back Office
---
