---
api_key_in:
- header
api_specs:
- filename: dinari-openapi-original.yml
  format: yaml
  label: Dinari Enterprise API
  slug: dinari-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-openapi-original.yml
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
- Stablecoin
- Fintech
- KYC
- Orders
- Wallets
---
