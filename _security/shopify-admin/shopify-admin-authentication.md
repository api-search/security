---
api_key_in:
- header
api_specs:
- filename: shopify-admin-rest-openapi.yml
  format: yaml
  label: Shopify Admin REST API
  slug: shopify-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify-admin/refs/heads/main/openapi/shopify-admin-rest-openapi.yml
- filename: shopify-admin-webhooks-asyncapi.yml
  format: yaml
  label: Shopify Webhooks
  slug: shopify-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify-admin/refs/heads/main/asyncapi/shopify-admin-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shopify Admin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shopify Admin API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shopify Admin API
provider_slug: shopify-admin
scheme_count: 1
schemes:
- description: Shopify access token for authentication
  in: header
  name: AccessToken
  parameter: X-Shopify-Access-Token
  sources:
  - openapi/shopify-admin-rest-openapi.yml
  type: apiKey
slug: shopify-admin-authentication
source_filename: shopify-admin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopify-admin-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: X-Shopify-Access-Token\n  description: Shopify access token for authentication\n  sources:\n  - openapi/shopify-admin-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopify-admin/refs/heads/main/authentication/shopify-admin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- Ecommerce
- Admin
- Products
- Orders
- Customers
---
