---
api_key_in: []
api_specs:
- filename: bybe-clips-api-openapi.yml
  format: yaml
  label: BYBE Clips API
  slug: bybe-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-clips-api-openapi.yml
- filename: bybe-consumers-api-openapi.yml
  format: yaml
  label: BYBE Consumers API
  slug: bybe-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-consumers-api-openapi.yml
- filename: bybe-manufacturers-api-openapi.yml
  format: yaml
  label: BYBE Manufacturers API
  slug: bybe-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-manufacturers-api-openapi.yml
- filename: bybe-offers-api-openapi.yml
  format: yaml
  label: BYBE Offers API
  slug: bybe-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-offers-api-openapi.yml
- filename: bybe-products-api-openapi.yml
  format: yaml
  label: BYBE Products API
  slug: bybe-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-products-api-openapi.yml
- filename: bybe-redemptions-api-openapi.yml
  format: yaml
  label: BYBE Redemptions API
  slug: bybe-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-redemptions-api-openapi.yml
- filename: bybe-stores-api-openapi.yml
  format: yaml
  label: BYBE Stores API
  slug: bybe-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/openapi/bybe-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bybe Authentication
name_suffix: Authentication
oauth_flows: []
overview: BYBE secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BYBE
provider_slug: bybe
scheme_count: 1
schemes:
- description: "Use your API key (token) and your API secret for username and password respectively.\n\n You can get these credentials, or generate new ones, on your developer page.\n\n You should encode your `Authorization:` header value in base64 as `api_key:api_secret`.\n (This will be shown as a curl request for you if you use the 'try it out' feature on this page while authorized.)"
  name: basic_auth
  scheme: basic
  sources:
  - openapi/bybe-api-openapi-original.yml
  type: http
slug: bybe-authentication
source_filename: bybe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/bybe-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: |-\n    Use your API key (token) and your API secret for username and password respectively.\n\n     You can get these credentials, or generate new ones, on your developer page.\n\n     You should encode your `Authorization:` header value in base64 as `api_key:api_secret`.\n     (This will be shown as a curl request for you if you use the 'try it out' feature on this page while authorized.)\n  sources:\n  - openapi/bybe-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/authentication/bybe-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Alcohol
- Beverages
- Promotions
- Rebates
- Marketing
- Retail
- CPG
- Loyalty
- Payments
- Disbursements
- Compliance
---
