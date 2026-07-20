---
api_key_in:
- header
api_specs:
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Platform API
  slug: codat-io-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Accounting API
  slug: codat-io-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Banking API
  slug: codat-io-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Commerce API
  slug: codat-io-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Lending API
  slug: codat-io-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Bank Feeds API
  slug: codat-io-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Sync for Payables API
  slug: codat-io-sync-for-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Sync for Expenses API
  slug: codat-io-sync-for-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Sync for Commerce API
  slug: codat-io-sync-for-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Codat Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codat secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codat
provider_slug: codat-io
scheme_count: 1
schemes:
- description: 'Codat expects your API key Base64-encoded and sent in the Authorization header using the Basic scheme, for example: `Authorization: Basic [example key]`.'
  in: header
  name: authHeader
  parameter: Authorization
  sources:
  - openapi/codat-io-openapi.yml
  type: apiKey
slug: codat-io-authentication
source_filename: codat-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codat-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Codat expects your API key Base64-encoded and sent in the Authorization header\n    using the Basic scheme, for example: `Authorization: Basic [example key]`.'\n  sources:\n  - openapi/codat-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/authentication/codat-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Data
- Accounting
- Banking
- Commerce
- Fintech
- Lending
- Financial Data
---
