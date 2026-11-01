---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: huuray-balance-api-openapi.yml
  format: yaml
  label: Huuray Balance API
  slug: huuray-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-balance-api-openapi.yml
- filename: huuray-cancel-api-openapi.yml
  format: yaml
  label: Huuray Cancel API
  slug: huuray-cancel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-cancel-api-openapi.yml
- filename: huuray-catalogue-api-openapi.yml
  format: yaml
  label: Huuray Catalogue API
  slug: huuray-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-catalogue-api-openapi.yml
- filename: huuray-order-api-openapi.yml
  format: yaml
  label: Huuray Order API
  slug: huuray-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-order-api-openapi.yml
- filename: huuray-resend-api-openapi.yml
  format: yaml
  label: Huuray Resend API
  slug: huuray-resend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-resend-api-openapi.yml
- filename: huuray-search-api-openapi.yml
  format: yaml
  label: Huuray Search API
  slug: huuray-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-search-api-openapi.yml
- filename: huuray-stock-api-openapi.yml
  format: yaml
  label: Huuray Stock API
  slug: huuray-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-stock-api-openapi.yml
- filename: huuray-template-api-openapi.yml
  format: yaml
  label: Huuray Template API
  slug: huuray-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-template-api-openapi.yml
- filename: huuray-exchange-rates-api-openapi.yml
  format: yaml
  label: Huuray Exchange Rates API
  slug: huuray-exchange-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/huuray/openapi/huuray-exchange-rates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Huuray Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huuray secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Huuray
provider_slug: huuray
scheme_count: 1
schemes:
- description: The API-Token provided to you by Huuray.
  in: header
  name: ApiToken
  parameter: X-API-TOKEN
  sources:
  - openapi/huuray-openapi.yml
  type: apiKey
slug: huuray-authentication
source_filename: huuray-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/huuray-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-API-TOKEN\n  description: The API-Token provided to you by Huuray.\n  sources:\n  - openapi/huuray-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/huuray/authentication/huuray-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Commerce
- Gift Cards
- Payments
- Rewards
---
