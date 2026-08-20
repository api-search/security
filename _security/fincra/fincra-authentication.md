---
api_key_in:
- header
api_specs:
- filename: fincra-account-resolution-api-openapi.yml
  format: yaml
  label: Fincra Account Resolution API
  slug: fincra-account-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-account-resolution-api-openapi.yml
- filename: fincra-banks-api-openapi.yml
  format: yaml
  label: Fincra Banks API
  slug: fincra-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-banks-api-openapi.yml
- filename: fincra-beneficiaries-api-openapi.yml
  format: yaml
  label: Fincra Beneficiaries API
  slug: fincra-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-beneficiaries-api-openapi.yml
- filename: fincra-collections-api-openapi.yml
  format: yaml
  label: Fincra Collections API
  slug: fincra-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-collections-api-openapi.yml
- filename: fincra-conversions-api-openapi.yml
  format: yaml
  label: Fincra Conversions API
  slug: fincra-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-conversions-api-openapi.yml
- filename: fincra-payouts-api-openapi.yml
  format: yaml
  label: Fincra Payouts API
  slug: fincra-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-payouts-api-openapi.yml
- filename: fincra-quotes-api-openapi.yml
  format: yaml
  label: Fincra Quotes API
  slug: fincra-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-quotes-api-openapi.yml
- filename: fincra-virtual-accounts-api-openapi.yml
  format: yaml
  label: Fincra Virtual Accounts API
  slug: fincra-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-virtual-accounts-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fincra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fincra secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fincra
provider_slug: fincra
scheme_count: 2
schemes:
- description: Merchant secret API key.
  in: header
  name: ApiKeyAuth
  parameter: api-key
  sources:
  - openapi/fincra-openapi.yml
  type: apiKey
- description: Bearer access token issued to the merchant.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fincra-openapi.yml
  type: http
slug: fincra-authentication
source_filename: fincra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fincra-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Merchant secret API key.\n  sources:\n  - openapi/fincra-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token issued to the merchant.\n  sources:\n  - openapi/fincra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/authentication/fincra-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Cross-Border
- Collection
- Payouts
- FX
- Fintech
- Africa
---
