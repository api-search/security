---
api_key_in:
- query
api_specs:
- filename: best-buy-products-api.yaml
  format: yaml
  label: Best Buy Products API
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-products-api.yaml
- filename: best-buy-stores-api.yaml
  format: yaml
  label: Best Buy Stores API
  slug: stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-stores-api.yaml
- filename: best-buy-recommendations-api.yaml
  format: yaml
  label: Best Buy Recommendations API
  slug: recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-recommendations-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Best Buy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Best Buy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Best Buy
provider_slug: best-buy
scheme_count: 1
schemes:
- description: API key obtained by registering at developer.bestbuy.com.
  in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/best-buy-products-api.yaml
  - openapi/best-buy-recommendations-api.yaml
  - openapi/best-buy-stores-api.yaml
  type: apiKey
slug: best-buy-authentication
source_filename: best-buy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/best-buy-products-api.yaml, openapi/best-buy-recommendations-api.yaml, openapi/best-buy-stores-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key obtained by registering at developer.bestbuy.com.\n  sources:\n  - openapi/best-buy-products-api.yaml\n  - openapi/best-buy-recommendations-api.yaml\n  - openapi/best-buy-stores-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/authentication/best-buy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fortune 100
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
---
