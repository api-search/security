---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fyndiq-articles-api-openapi.yml
  format: yaml
  label: Fyndiq Articles API
  slug: fyndiq-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-articles-api-openapi.yml
- filename: fyndiq-orders-api-openapi.yml
  format: yaml
  label: Fyndiq Orders API
  slug: fyndiq-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-orders-api-openapi.yml
- filename: fyndiq-carrier-codes-api-openapi.yml
  format: yaml
  label: Fyndiq Carrier Codes API
  slug: fyndiq-carrier-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-carrier-codes-api-openapi.yml
- filename: fyndiq-categories-api-openapi.yml
  format: yaml
  label: Fyndiq Categories API
  slug: fyndiq-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-categories-api-openapi.yml
- filename: fyndiq-financial-reports-api-openapi.yml
  format: yaml
  label: Fyndiq Financial Reports API
  slug: fyndiq-financial-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-financial-reports-api-openapi.yml
- filename: fyndiq-health-api-openapi.yml
  format: yaml
  label: Fyndiq Health API
  slug: fyndiq-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-health-api-openapi.yml
- filename: fyndiq-jobs-api-openapi.yml
  format: yaml
  label: Fyndiq Jobs API
  slug: fyndiq-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-jobs-api-openapi.yml
- filename: fyndiq-merchant-api-openapi.yml
  format: yaml
  label: Fyndiq Merchant API
  slug: fyndiq-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-merchant-api-openapi.yml
- filename: fyndiq-sales-funnels-api-openapi.yml
  format: yaml
  label: Fyndiq Sales Funnels API
  slug: fyndiq-sales-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-sales-funnels-api-openapi.yml
- filename: fyndiq-shipping-configurations-api-openapi.yml
  format: yaml
  label: Fyndiq Shipping Configurations API
  slug: fyndiq-shipping-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-shipping-configurations-api-openapi.yml
- filename: fyndiq-statuses-api-openapi.yml
  format: yaml
  label: Fyndiq Statuses API
  slug: fyndiq-statuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-statuses-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fyndiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fyndiq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fyndiq
provider_slug: fyndiq
scheme_count: 1
schemes:
- description: Base64-encoded `merchantID:token`.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fyndiq-merchant-api-openapi.yml
  type: http
slug: fyndiq-authentication
source_filename: fyndiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/fyndiq-merchant-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64-encoded `merchantID:token`.\n  sources:\n  - openapi/fyndiq-merchant-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fyndiq/authentication/fyndiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Marketplace
- E-Commerce
- Retail
- Product
- Order
- Sweden
---
