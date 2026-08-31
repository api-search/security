---
api_key_in:
- header
api_specs:
- filename: helcim-ach-payment-api-openapi.yml
  format: yaml
  label: Helcim ACH Payment API
  slug: helcim-ach-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-ach-payment-api-openapi.yml
- filename: helcim-card-batch-api-openapi.yml
  format: yaml
  label: Helcim Card Batch API
  slug: helcim-card-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-card-batch-api-openapi.yml
- filename: helcim-card-terminal-api-openapi.yml
  format: yaml
  label: Helcim Card Terminal API
  slug: helcim-card-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-card-terminal-api-openapi.yml
- filename: helcim-card-transaction-api-openapi.yml
  format: yaml
  label: Helcim Card Transaction API
  slug: helcim-card-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-card-transaction-api-openapi.yml
- filename: helcim-customer-api-openapi.yml
  format: yaml
  label: Helcim Customer API
  slug: helcim-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-customer-api-openapi.yml
- filename: helcim-device-api-openapi.yml
  format: yaml
  label: Helcim Device API
  slug: helcim-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-device-api-openapi.yml
- filename: helcim-general-api-openapi.yml
  format: yaml
  label: Helcim General API
  slug: helcim-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-general-api-openapi.yml
- filename: helcim-invoice-api-openapi.yml
  format: yaml
  label: Helcim Invoice API
  slug: helcim-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-invoice-api-openapi.yml
- filename: helcim-payment-api-openapi.yml
  format: yaml
  label: Helcim Payment API
  slug: helcim-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-payment-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Helcim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helcim secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Helcim
provider_slug: helcim
scheme_count: 1
schemes:
- description: API Token with required permissions
  in: header
  name: ApiAccessAuth
  parameter: api-token
  sources:
  - openapi/helcim-api.json
  type: apiKey
slug: helcim-authentication
source_filename: helcim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/helcim-api.json + https://devdocs.helcim.com/docs/authentication-with-the-helcim-api-and-helcimpayjs\ndocs: https://devdocs.helcim.com/docs/authentication-with-the-helcim-api-and-helcimpayjs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nmodel: Permissioned API access token created per API Access Configuration in the Helcim dashboard. Each\n  token carries granular per-resource permissions (e.g. General, Processing, Settings set to Read / PositiveTransaction\n  / Admin) which gate individual operations.\nschemes:\n- name: ApiAccessAuth\n  type: apiKey\n  in: header\n  parameter: api-token\n  description: API Token with required permissions\n  sources:\n  - openapi/helcim-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/authentication/helcim-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Canada
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- ACH
- Invoicing
- Card Terminal
- Small Business
---
