---
api_key_in:
- header
api_specs:
- filename: amazon-seller-central-openapi.yml
  format: yaml
  label: Amazon Selling Partner API (SP-API)
  slug: sp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-seller-central/refs/heads/main/openapi/amazon-seller-central-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Seller Central Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Selling Partner API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Selling Partner API
provider_slug: amazon-seller-central
scheme_count: 1
schemes:
- description: Login with Amazon (LWA) OAuth 2.0 access token.
  in: header
  name: LwaBearer
  parameter: x-amz-access-token
  sources:
  - openapi/amazon-seller-central-openapi.yml
  type: apiKey
slug: amazon-seller-central-authentication
source_filename: amazon-seller-central-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-seller-central-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LwaBearer\n  type: apiKey\n  in: header\n  parameter: x-amz-access-token\n  description: Login with Amazon (LWA) OAuth 2.0 access token.\n  sources:\n  - openapi/amazon-seller-central-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-seller-central/refs/heads/main/authentication/amazon-seller-central-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- eCommerce
- Marketplace
- Selling Partner
- Amazon
- Seller Central
- Catalog
- Orders
- Inventory
- Fulfillment
---
