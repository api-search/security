---
api_key_in:
- header
api_specs:
- filename: shopup-redx-openapi.yml
  format: yaml
  label: REDX Open API
  slug: redx-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopup/refs/heads/main/openapi/shopup-redx-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shopup Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShopUp secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ShopUp
provider_slug: shopup
scheme_count: 1
schemes:
- description: 'Merchant access token, sent as: API-ACCESS-TOKEN: Bearer {jwt_token}'
  in: header
  name: apiAccessToken
  parameter: API-ACCESS-TOKEN
  sources:
  - openapi/shopup-redx-openapi.yml
  type: apiKey
slug: shopup-authentication
source_filename: shopup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/shopup-redx-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiAccessToken\n  type: apiKey\n  in: header\n  parameter: API-ACCESS-TOKEN\n  description: 'Merchant access token, sent as: API-ACCESS-TOKEN: Bearer {jwt_token}'\n  sources:\n  - openapi/shopup-redx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopup/refs/heads/main/authentication/shopup-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketplace
- Logistics
- Courier
- Last Mile Delivery
- B2B Commerce
- Bangladesh
- E-commerce
- Fintech
---
