---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: istock-countries-api-openapi.yml
  format: yaml
  label: iStock Countries API
  slug: istock-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-countries-api-openapi.yml
- filename: istock-downloads-api-openapi.yml
  format: yaml
  label: iStock Downloads API
  slug: istock-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-downloads-api-openapi.yml
- filename: istock-images-api-openapi.yml
  format: yaml
  label: iStock Images API
  slug: istock-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-images-api-openapi.yml
- filename: istock-search-api-openapi.yml
  format: yaml
  label: iStock Search API
  slug: istock-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-search-api-openapi.yml
- filename: istock-videos-api-openapi.yml
  format: yaml
  label: iStock Videos API
  slug: istock-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-videos-api-openapi.yml
- filename: istock-affiliatesearch-api-openapi.yml
  format: yaml
  label: iStock Affiliate Search API
  slug: istock-affiliatesearch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-affiliatesearch-api-openapi.yml
- filename: istock-aigenerator-api-openapi.yml
  format: yaml
  label: iStock AI Generator API
  slug: istock-aigenerator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-aigenerator-api-openapi.yml
- filename: istock-artists-api-openapi.yml
  format: yaml
  label: iStock Artists API
  slug: istock-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-artists-api-openapi.yml
- filename: istock-assetchanges-api-openapi.yml
  format: yaml
  label: iStock Asset Changes API
  slug: istock-assetchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-assetchanges-api-openapi.yml
- filename: istock-assetlicensing-api-openapi.yml
  format: yaml
  label: iStock Asset Licensing API
  slug: istock-assetlicensing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-assetlicensing-api-openapi.yml
- filename: istock-boards-api-openapi.yml
  format: yaml
  label: iStock Boards API
  slug: istock-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-boards-api-openapi.yml
- filename: istock-collections-api-openapi.yml
  format: yaml
  label: iStock Collections API
  slug: istock-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-collections-api-openapi.yml
- filename: istock-customers-api-openapi.yml
  format: yaml
  label: iStock Customers API
  slug: istock-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-customers-api-openapi.yml
- filename: istock-events-api-openapi.yml
  format: yaml
  label: iStock Events API
  slug: istock-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-events-api-openapi.yml
- filename: istock-imagematch-api-openapi.yml
  format: yaml
  label: iStock Image Match API
  slug: istock-imagematch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-imagematch-api-openapi.yml
- filename: istock-orders-api-openapi.yml
  format: yaml
  label: iStock Orders API
  slug: istock-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-orders-api-openapi.yml
- filename: istock-products-api-openapi.yml
  format: yaml
  label: iStock Products API
  slug: istock-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-products-api-openapi.yml
- filename: istock-purchases-api-openapi.yml
  format: yaml
  label: iStock Purchases API
  slug: istock-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-purchases-api-openapi.yml
- filename: istock-usage-api-openapi.yml
  format: yaml
  label: iStock Usage API
  slug: istock-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-usage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Istock Authentication
name_suffix: Authentication
oauth_flows: []
overview: iStock secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: iStock
provider_slug: istock
scheme_count: 2
schemes:
- description: API key issued through the Getty Images developer program.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/istock-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via /oauth2/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/istock-openapi.yml
  type: http
slug: istock-authentication
source_filename: istock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/istock-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key issued through the Getty Images developer program.\n  sources:\n  - openapi/istock-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via /oauth2/token.\n  sources:\n  - openapi/istock-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/istock/authentication/istock-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Stock Media
- Image
- Video
- Illustrations
- Royalty-Free
- Getty
---
