---
api_key_in:
- header
api_specs:
- filename: mealme-openapi.yml
  format: yaml
  label: MealMe Food Ordering API
  slug: mealme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-openapi.yml
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
