---
api_key_in:
- header
api_specs:
- filename: plug-3ds2-malga-api-openapi.yml
  format: yaml
  label: Malga 3DS2 Malga API
  slug: plug-3ds2-malga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-3ds2-malga-api-openapi.yml
- filename: plug-cards-api-openapi.yml
  format: yaml
  label: Malga Cards API
  slug: plug-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-cards-api-openapi.yml
- filename: plug-charges-api-openapi.yml
  format: yaml
  label: Malga Charges API
  slug: plug-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-charges-api-openapi.yml
- filename: plug-client-token-api-openapi.yml
  format: yaml
  label: Malga Client-token API
  slug: plug-client-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-client-token-api-openapi.yml
- filename: plug-customers-api-openapi.yml
  format: yaml
  label: Malga Customers API
  slug: plug-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-customers-api-openapi.yml
- filename: plug-flows-api-openapi.yml
  format: yaml
  label: Malga Flows API
  slug: plug-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-flows-api-openapi.yml
- filename: plug-merchants-api-openapi.yml
  format: yaml
  label: Malga Merchants API
  slug: plug-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-merchants-api-openapi.yml
- filename: plug-payouts-api-openapi.yml
  format: yaml
  label: Malga Payouts API
  slug: plug-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-payouts-api-openapi.yml
- filename: plug-prepayment-api-openapi.yml
  format: yaml
  label: Malga Prepayment API
  slug: plug-prepayment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-prepayment-api-openapi.yml
- filename: plug-providers-api-openapi.yml
  format: yaml
  label: Malga Providers API
  slug: plug-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-providers-api-openapi.yml
- filename: plug-seller-documents-api-openapi.yml
  format: yaml
  label: Malga Seller Documents API
  slug: plug-seller-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-seller-documents-api-openapi.yml
- filename: plug-sellers-api-openapi.yml
  format: yaml
  label: Malga Sellers API
  slug: plug-sellers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-sellers-api-openapi.yml
- filename: plug-sessions-api-openapi.yml
  format: yaml
  label: Malga Sessions API
  slug: plug-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-sessions-api-openapi.yml
- filename: plug-settings-api-openapi.yml
  format: yaml
  label: Malga Settings API
  slug: plug-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-settings-api-openapi.yml
- filename: plug-subscriptions-api-openapi.yml
  format: yaml
  label: Malga Subscriptions API
  slug: plug-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-subscriptions-api-openapi.yml
- filename: plug-tokens-api-openapi.yml
  format: yaml
  label: Malga Tokens API
  slug: plug-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-tokens-api-openapi.yml
- filename: plug-vendors-api-openapi.yml
  format: yaml
  label: Malga Vendors API
  slug: plug-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-vendors-api-openapi.yml
- filename: plug-webhooks-api-openapi.yml
  format: yaml
  label: Malga Webhooks API
  slug: plug-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Plug Authentication
name_suffix: Authentication
oauth_flows: []
overview: Malga secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Malga
provider_slug: plug
scheme_count: 2
schemes:
- in: header
  name: X-Client-ID
  parameter: X-Client-Id
  sources:
  - openapi/plug-openapi-original.yml
  type: apiKey
- in: header
  name: X-Api-Key
  parameter: X-Api-Key
  sources:
  - openapi/plug-openapi-original.yml
  type: apiKey
slug: plug-authentication
source_filename: plug-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/plug-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Client-ID\n  type: apiKey\n  in: header\n  parameter: X-Client-Id\n  sources:\n  - openapi/plug-openapi-original.yml\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/plug-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/authentication/plug-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Payment Orchestration
- Payment Gateway
- Fintech
- Pix
- Tokenization
- Subscription
- Brazil
---
