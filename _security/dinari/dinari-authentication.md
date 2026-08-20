---
api_key_in:
- header
api_specs:
- filename: dinari-accounts-api-openapi.yml
  format: yaml
  label: Dinari Accounts API
  slug: dinari-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-accounts-api-openapi.yml
- filename: dinari-corporate-actions-api-openapi.yml
  format: yaml
  label: Dinari Corporate Actions API
  slug: dinari-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-corporate-actions-api-openapi.yml
- filename: dinari-entities-api-openapi.yml
  format: yaml
  label: Dinari Entities API
  slug: dinari-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-entities-api-openapi.yml
- filename: dinari-kyc-api-openapi.yml
  format: yaml
  label: Dinari KYC API
  slug: dinari-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-kyc-api-openapi.yml
- filename: dinari-managed-orders-api-openapi.yml
  format: yaml
  label: Dinari Managed Orders API
  slug: dinari-managed-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-managed-orders-api-openapi.yml
- filename: dinari-market-data-api-openapi.yml
  format: yaml
  label: Dinari Market Data API
  slug: dinari-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-market-data-api-openapi.yml
- filename: dinari-order-requests-api-openapi.yml
  format: yaml
  label: Dinari Order Requests API
  slug: dinari-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-order-requests-api-openapi.yml
- filename: dinari-orders-api-openapi.yml
  format: yaml
  label: Dinari Orders API
  slug: dinari-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-orders-api-openapi.yml
- filename: dinari-wallets-api-openapi.yml
  format: yaml
  label: Dinari Wallets API
  slug: dinari-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-wallets-api-openapi.yml
- filename: dinari-withdrawals-api-openapi.yml
  format: yaml
  label: Dinari Withdrawals API
  slug: dinari-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-withdrawals-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dinari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dinari secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dinari
provider_slug: dinari
scheme_count: 2
schemes:
- description: The API key ID provided on the [Partners Dashboard](https://partners.dinari.com).
  in: header
  name: ApiKeyId
  parameter: X-API-Key-Id
  sources:
  - openapi/dinari-openapi-original.yml
  type: apiKey
- description: API Secret Key that is only shown once at API Key creation.
  in: header
  name: ApiSecretKey
  parameter: X-API-Secret-Key
  sources:
  - openapi/dinari-openapi-original.yml
  type: apiKey
slug: dinari-authentication
source_filename: dinari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dinari-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyId\n  type: apiKey\n  in: header\n  parameter: X-API-Key-Id\n  description: The API key ID provided on the [Partners Dashboard](https://partners.dinari.com).\n  sources:\n  - openapi/dinari-openapi-original.yml\n- name: ApiSecretKey\n  type: apiKey\n  in: header\n  parameter: X-API-Secret-Key\n  description: API Secret Key that is only shown once at API Key creation.\n  sources:\n  - openapi/dinari-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/authentication/dinari-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Tokenized Securities
- Stocks
- ETFs
- Brokerage
- Market Data
- Blockchain
- Stablecoins
- Fintech
- KYC
- Order
- Wallets
---
