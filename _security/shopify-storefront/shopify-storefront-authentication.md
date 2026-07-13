---
api_key_in:
- header
api_specs:
- filename: shopify-storefront-openapi.yml
  format: yaml
  label: Shopify Storefront API
  slug: shopify-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify-storefront/refs/heads/main/openapi/shopify-storefront-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shopify Storefront Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shopify Storefront API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shopify Storefront API
provider_slug: shopify-storefront
scheme_count: 1
schemes:
- description: Public Storefront API access token for the store
  in: header
  name: StorefrontAccessToken
  parameter: X-Shopify-Storefront-Access-Token
  sources:
  - openapi/shopify-storefront-openapi.yml
  type: apiKey
slug: shopify-storefront-authentication
source_filename: shopify-storefront-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopify-storefront-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: StorefrontAccessToken\n  type: apiKey\n  in: header\n  parameter: X-Shopify-Storefront-Access-Token\n  description: Public Storefront API access token for the store\n  sources:\n  - openapi/shopify-storefront-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopify-storefront/refs/heads/main/authentication/shopify-storefront-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- Ecommerce
- Headless
- GraphQL
- Storefront
- Products
- Cart
- Checkout
---
