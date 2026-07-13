---
api_key_in:
- header
api_specs:
- filename: shopify-api-openapi.yml
  format: yaml
  label: Shopify Admin REST API
  slug: shopify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-api-openapi.yml
- filename: shopify-ajax-api-openapi.yml
  format: yaml
  label: Shopify Ajax API
  slug: ajax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-ajax-api-openapi.yml
- filename: shopify-webhooks-api-openapi.yml
  format: yaml
  label: Shopify Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-webhooks-api-openapi.yml
- filename: shopify-multipass-api-openapi.yml
  format: yaml
  label: Shopify Multipass API
  slug: multipass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-multipass-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shopify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shopify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shopify
provider_slug: shopify
scheme_count: 1
schemes:
- description: Access token obtained via OAuth
  in: header
  name: AccessToken
  parameter: X-Shopify-Access-Token
  sources:
  - openapi/shopify-admin-rest-api-openapi.yml
  - openapi/shopify-webhooks-api-openapi.yml
  type: apiKey
slug: shopify-authentication
source_filename: shopify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopify-admin-rest-api-openapi.yml, openapi/shopify-webhooks-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: X-Shopify-Access-Token\n  description: Access token obtained via OAuth\n  sources:\n  - openapi/shopify-admin-rest-api-openapi.yml\n  - openapi/shopify-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/authentication/shopify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
---
