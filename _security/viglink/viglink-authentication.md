---
api_key_in:
- header
api_specs:
- filename: viglink-link-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Link Check API
  slug: link-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-check-openapi.yml
- filename: viglink-bid-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Bid Check API
  slug: bid-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-check-openapi.yml
- filename: viglink-campaigns-openapi.yml
  format: yaml
  label: Sovrn Commerce Campaigns API
  slug: campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-campaigns-openapi.yml
- filename: viglink-reports-openapi.yml
  format: yaml
  label: Sovrn Commerce Real-Time Reports API
  slug: real-time-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-openapi.yml
- filename: viglink-merchant-summaries-openapi.yml
  format: yaml
  label: Sovrn Commerce Merchant Group Summaries API
  slug: merchant-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-summaries-openapi.yml
- filename: viglink-product-recommendations-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Recommendations API
  slug: product-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-recommendations-openapi.yml
- filename: viglink-product-promo-codes-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Promo Codes API
  slug: product-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-promo-codes-openapi.yml
- filename: viglink-price-comparisons-openapi.yml
  format: yaml
  label: Sovrn Commerce Price Comparisons API
  slug: price-comparisons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-price-comparisons-openapi.yml
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
