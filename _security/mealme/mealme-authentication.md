---
api_key_in:
- header
api_specs:
- filename: mealme-carts-api-openapi.yml
  format: yaml
  label: MealMe Carts API
  slug: mealme-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-carts-api-openapi.yml
- filename: mealme-connect-accounts-api-openapi.yml
  format: yaml
  label: MealMe Connect Accounts API
  slug: mealme-connect-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-connect-accounts-api-openapi.yml
- filename: mealme-geocoding-api-openapi.yml
  format: yaml
  label: MealMe Geocoding API
  slug: mealme-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-geocoding-api-openapi.yml
- filename: mealme-orders-api-openapi.yml
  format: yaml
  label: MealMe Orders API
  slug: mealme-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-orders-api-openapi.yml
- filename: mealme-payments-api-openapi.yml
  format: yaml
  label: MealMe Payments API
  slug: mealme-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-payments-api-openapi.yml
- filename: mealme-search-api-openapi.yml
  format: yaml
  label: MealMe Search API
  slug: mealme-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-search-api-openapi.yml
- filename: mealme-stores-api-openapi.yml
  format: yaml
  label: MealMe Stores API
  slug: mealme-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-stores-api-openapi.yml
- filename: mealme-support-chat-api-openapi.yml
  format: yaml
  label: MealMe Support Chat API
  slug: mealme-support-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-support-chat-api-openapi.yml
- filename: mealme-tracking-api-openapi.yml
  format: yaml
  label: MealMe Tracking API
  slug: mealme-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-tracking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mealme Authentication
name_suffix: Authentication
oauth_flows: []
overview: MealMe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MealMe
provider_slug: mealme
scheme_count: 1
schemes:
- description: API key issued by MealMe, passed in the Authorization header.
  in: header
  name: apiKeyHeader
  parameter: Authorization
  sources:
  - openapi/mealme-openapi.yml
  type: apiKey
slug: mealme-authentication
source_filename: mealme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mealme-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key issued by MealMe, passed in the Authorization header.\n  sources:\n  - openapi/mealme-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/authentication/mealme-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Delivery
- Food
- Grocery
- Ordering
- Restaurants
---
