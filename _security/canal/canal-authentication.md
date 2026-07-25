---
api_key_in:
- header
api_specs:
- filename: canal-csv-api-openapi.yml
  format: yaml
  label: Canal csv API
  slug: canal-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-csv-api-openapi.yml
- filename: canal-fulfillments-api-openapi.yml
  format: yaml
  label: Canal fulfillments API
  slug: canal-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-fulfillments-api-openapi.yml
- filename: canal-markets-api-openapi.yml
  format: yaml
  label: Canal markets API
  slug: canal-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-markets-api-openapi.yml
- filename: canal-max-shipping-rates-api-openapi.yml
  format: yaml
  label: Canal max-shipping-rates API
  slug: canal-max-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-max-shipping-rates-api-openapi.yml
- filename: canal-orders-api-openapi.yml
  format: yaml
  label: Canal orders API
  slug: canal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-orders-api-openapi.yml
- filename: canal-product-sets-api-openapi.yml
  format: yaml
  label: Canal product_sets API
  slug: canal-product-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-product-sets-api-openapi.yml
- filename: canal-products-api-openapi.yml
  format: yaml
  label: Canal products API
  slug: canal-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-products-api-openapi.yml
- filename: canal-refunds-api-openapi.yml
  format: yaml
  label: Canal refunds API
  slug: canal-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-refunds-api-openapi.yml
- filename: canal-returns-api-openapi.yml
  format: yaml
  label: Canal returns API
  slug: canal-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-returns-api-openapi.yml
- filename: canal-selection-api-openapi.yml
  format: yaml
  label: Canal selection API
  slug: canal-selection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-selection-api-openapi.yml
- filename: canal-shipping-api-openapi.yml
  format: yaml
  label: Canal shipping API
  slug: canal-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-shipping-api-openapi.yml
- filename: canal-shipping-rates-api-openapi.yml
  format: yaml
  label: Canal shipping-rates API
  slug: canal-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-shipping-rates-api-openapi.yml
- filename: canal-shops-api-openapi.yml
  format: yaml
  label: Canal shops API
  slug: canal-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-shops-api-openapi.yml
- filename: canal-tax-and-shipping-api-openapi.yml
  format: yaml
  label: Canal tax-and-shipping API
  slug: canal-tax-and-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-tax-and-shipping-api-openapi.yml
- filename: canal-tax-api-openapi.yml
  format: yaml
  label: Canal tax API
  slug: canal-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-tax-api-openapi.yml
- filename: canal-variants-api-openapi.yml
  format: yaml
  label: Canal variants API
  slug: canal-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-variants-api-openapi.yml
- filename: canal-webhooks-api-openapi.yml
  format: yaml
  label: Canal webhooks API
  slug: canal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Canal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canal secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canal
provider_slug: canal
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/canal-openapi-original.yml
  type: http
- in: header
  name: platformAppId
  parameter: X-CANAL-APP-ID
  sources:
  - openapi/canal-openapi-original.yml
  type: apiKey
- in: header
  name: platformAppToken
  parameter: X-CANAL-APP-TOKEN
  sources:
  - openapi/canal-openapi-original.yml
  type: apiKey
slug: canal-authentication
source_filename: canal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/canal-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/canal-openapi-original.yml\n- name: platformAppId\n  type: apiKey\n  in: header\n  parameter: X-CANAL-APP-ID\n  sources:\n  - openapi/canal-openapi-original.yml\n- name: platformAppToken\n  type: apiKey\n  in: header\n  parameter: X-CANAL-APP-TOKEN\n  sources:\n  - openapi/canal-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/authentication/canal-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- eCommerce
- Dropshipping
- Marketplace
- Commerce
- Retail
- Fulfillment
- Orders
- Products
- Webhooks
---
