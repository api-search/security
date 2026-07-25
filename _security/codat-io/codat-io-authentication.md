---
api_key_in:
- header
api_specs:
- filename: codat-io-accounting-api-openapi.yml
  format: yaml
  label: Codat Accounting API
  slug: codat-io-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-accounting-api-openapi.yml
- filename: codat-io-bank-feeds-api-openapi.yml
  format: yaml
  label: Codat Bank Feeds API
  slug: codat-io-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-bank-feeds-api-openapi.yml
- filename: codat-io-banking-api-openapi.yml
  format: yaml
  label: Codat Banking API
  slug: codat-io-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-banking-api-openapi.yml
- filename: codat-io-commerce-api-openapi.yml
  format: yaml
  label: Codat Commerce API
  slug: codat-io-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-commerce-api-openapi.yml
- filename: codat-io-companies-api-openapi.yml
  format: yaml
  label: Codat Companies API
  slug: codat-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-companies-api-openapi.yml
- filename: codat-io-connections-api-openapi.yml
  format: yaml
  label: Codat Connections API
  slug: codat-io-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-connections-api-openapi.yml
- filename: codat-io-expenses-api-openapi.yml
  format: yaml
  label: Codat Expenses API
  slug: codat-io-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-expenses-api-openapi.yml
- filename: codat-io-integrations-api-openapi.yml
  format: yaml
  label: Codat Integrations API
  slug: codat-io-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-integrations-api-openapi.yml
- filename: codat-io-lending-api-openapi.yml
  format: yaml
  label: Codat Lending API
  slug: codat-io-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-lending-api-openapi.yml
- filename: codat-io-manage-data-api-openapi.yml
  format: yaml
  label: Codat Manage data API
  slug: codat-io-manage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-manage-data-api-openapi.yml
- filename: codat-io-payables-api-openapi.yml
  format: yaml
  label: Codat Payables API
  slug: codat-io-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-payables-api-openapi.yml
- filename: codat-io-sync-for-commerce-api-openapi.yml
  format: yaml
  label: Codat Sync for Commerce API
  slug: codat-io-sync-for-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-sync-for-commerce-api-openapi.yml
- filename: codat-io-webhooks-api-openapi.yml
  format: yaml
  label: Codat Webhooks API
  slug: codat-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-webhooks-api-openapi.yml
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
