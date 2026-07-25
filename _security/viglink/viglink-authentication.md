---
api_key_in:
- header
api_specs:
- filename: viglink-account-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Account API
  slug: viglink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-account-api-openapi.yml
- filename: viglink-ai-orchestration-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Ai Orchestration API
  slug: viglink-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-ai-orchestration-api-openapi.yml
- filename: viglink-bid-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Bid API
  slug: viglink-bid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-api-openapi.yml
- filename: viglink-link-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Link API
  slug: viglink-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-api-openapi.yml
- filename: viglink-merchant-group-summaries-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Merchant Group Summaries API
  slug: viglink-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-group-summaries-api-openapi.yml
- filename: viglink-product-coupons-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Product Coupons API
  slug: viglink-product-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-coupons-api-openapi.yml
- filename: viglink-reports-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) reports API
  slug: viglink-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-api-openapi.yml
- filename: viglink-sites-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Sites API
  slug: viglink-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-sites-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Viglink Authentication
name_suffix: Authentication
oauth_flows: []
overview: VigLink (Sovrn Commerce) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VigLink (Sovrn Commerce)
provider_slug: viglink
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: authorization
  sources:
  - openapi/viglink-campaigns-openapi.yml
  - openapi/viglink-price-comparisons-openapi.yml
  - openapi/viglink-reports-openapi.yml
  type: apiKey
- description: 'Authorization header using the Secret Key scheme. Format: "secret {secret key}"'
  in: header
  name: SecretKey
  parameter: Authorization
  sources:
  - openapi/viglink-merchant-summaries-openapi.yml
  - openapi/viglink-product-promo-codes-openapi.yml
  type: apiKey
slug: viglink-authentication
source_filename: viglink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/viglink-campaigns-openapi.yml, openapi/viglink-merchant-summaries-openapi.yml,\n  openapi/viglink-price-comparisons-openapi.yml, openapi/viglink-product-promo-codes-openapi.yml,\n  openapi/viglink-reports-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/viglink-campaigns-openapi.yml\n  - openapi/viglink-price-comparisons-openapi.yml\n  - openapi/viglink-reports-openapi.yml\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authorization header using the Secret Key scheme. Format: \"secret {secret key}\"'\n  sources:\n  - openapi/viglink-merchant-summaries-openapi.yml\n  - openapi/viglink-product-promo-codes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/authentication/viglink-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Affiliate Marketing
- Commerce
- Monetization
- Publishers
- Links
- Advertising
- Reporting
---
