---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ecomscout-com-analytics-api-openapi.yml
  format: yaml
  label: EcomScout Analytics API
  slug: ecomscout-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-analytics-api-openapi.yml
- filename: ecomscout-com-apps-api-openapi.yml
  format: yaml
  label: EcomScout Apps API
  slug: ecomscout-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-apps-api-openapi.yml
- filename: ecomscout-com-audiences-api-openapi.yml
  format: yaml
  label: EcomScout Audiences API
  slug: ecomscout-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-audiences-api-openapi.yml
- filename: ecomscout-com-changes-api-openapi.yml
  format: yaml
  label: EcomScout Changes API
  slug: ecomscout-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-changes-api-openapi.yml
- filename: ecomscout-com-discovery-api-openapi.yml
  format: yaml
  label: EcomScout Discovery API
  slug: ecomscout-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-discovery-api-openapi.yml
- filename: ecomscout-com-products-api-openapi.yml
  format: yaml
  label: EcomScout Products API
  slug: ecomscout-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-products-api-openapi.yml
- filename: ecomscout-com-scrapes-api-openapi.yml
  format: yaml
  label: EcomScout Scrapes API
  slug: ecomscout-com-scrapes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-scrapes-api-openapi.yml
- filename: ecomscout-com-signals-api-openapi.yml
  format: yaml
  label: EcomScout Signals API
  slug: ecomscout-com-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-signals-api-openapi.yml
- filename: ecomscout-com-stores-api-openapi.yml
  format: yaml
  label: EcomScout Stores API
  slug: ecomscout-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-stores-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: EcomScout Authentication
name_suffix: Authentication
oauth_flows: []
overview: EcomScout secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EcomScout
provider_slug: ecomscout-com
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/ecomscout-com-openapi.json
  type: apiKey
- name: bearer
  scheme: bearer
  sources:
  - openapi/ecomscout-com-openapi.json
  type: http
slug: ecomscout-com-authentication
source_filename: ecomscout-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/ecomscout-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ecomscout-com-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ecomscout-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ecomscout-com/authentication/ecomscout-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Shopify
- Analytics
- E-Commerce
- Data
---
