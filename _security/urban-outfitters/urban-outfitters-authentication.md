---
api_key_in:
- header
api_specs:
- filename: urban-outfitters-affiliate-api-openapi.yml
  format: yaml
  label: Urban Outfitters Affiliate Program
  slug: affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-affiliate-api-openapi.yml
- filename: urban-outfitters-marketplace-api-openapi.yml
  format: yaml
  label: Urban Outfitters Marketplace (UO MRKT) Integration
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-marketplace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Urban Outfitters Authentication
name_suffix: Authentication
oauth_flows: []
overview: Urban Outfitters secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Urban Outfitters
provider_slug: urban-outfitters
scheme_count: 2
schemes:
- description: Rakuten Advertising API key provided upon affiliate program enrollment. Include as Bearer token in the Authorization header.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/urban-outfitters-affiliate-api-openapi.yml
  type: apiKey
- description: Seller API key provided by Urban Outfitters marketplace onboarding
  in: header
  name: apiKeyAuth
  parameter: X-Seller-API-Key
  sources:
  - openapi/urban-outfitters-marketplace-api-openapi.yml
  type: apiKey
slug: urban-outfitters-authentication
source_filename: urban-outfitters-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/urban-outfitters-affiliate-api-openapi.yml, openapi/urban-outfitters-marketplace-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Rakuten Advertising API key provided upon affiliate program enrollment. Include\n    as Bearer token in the Authorization header.\n  sources:\n  - openapi/urban-outfitters-affiliate-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Seller-API-Key\n  description: Seller API key provided by Urban Outfitters marketplace onboarding\n  sources:\n  - openapi/urban-outfitters-marketplace-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/authentication/urban-outfitters-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Retail
- Fashion
- Apparel
- Ecommerce
- Affiliate
- Marketplace
- Fortune 1000
---
