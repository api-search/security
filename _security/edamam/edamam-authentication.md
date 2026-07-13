---
api_key_in:
- query
api_specs:
- filename: edamam-nutrition-analysis-api-openapi.yml
  format: yaml
  label: Edamam Nutrition Analysis API
  slug: edamam-nutrition-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-nutrition-analysis-api-openapi.yml
- filename: edamam-food-and-grocery-database-api-openapi.yml
  format: yaml
  label: Edamam Food and Grocery Database API
  slug: edamam-food-and-grocery-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-food-and-grocery-database-api-openapi.yml
- filename: edamam-recipe-search-api-openapi.yml
  format: yaml
  label: Edamam Recipe Search API
  slug: edamam-recipe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-recipe-search-api-openapi.yml
- filename: edamam-meal-planner-api-openapi.yml
  format: yaml
  label: Edamam Meal Planner API
  slug: edamam-meal-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-meal-planner-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Edamam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edamam secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Edamam
provider_slug: edamam
scheme_count: 2
schemes:
- description: App key issued by Edamam. Must be sent with the matching `app_id` query parameter.
  in: query
  name: AppCreds
  parameter: app_key
  sources:
  - openapi/edamam-food-and-grocery-database-api-openapi.yml
  - openapi/edamam-nutrition-analysis-api-openapi.yml
  - openapi/edamam-recipe-search-api-openapi.yml
  type: apiKey
- description: HTTP Basic authentication using your Edamam app_id as username and app_key as password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/edamam-meal-planner-api-openapi.yml
  type: http
slug: edamam-authentication
source_filename: edamam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/edamam-food-and-grocery-database-api-openapi.yml, openapi/edamam-meal-planner-api-openapi.yml,\n  openapi/edamam-nutrition-analysis-api-openapi.yml, openapi/edamam-recipe-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: AppCreds\n  type: apiKey\n  in: query\n  parameter: app_key\n  description: App key issued by Edamam. Must be sent with the matching `app_id` query parameter.\n  sources:\n  - openapi/edamam-food-and-grocery-database-api-openapi.yml\n  - openapi/edamam-nutrition-analysis-api-openapi.yml\n  - openapi/edamam-recipe-search-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your Edamam app_id as username and app_key as\n    password.\n  sources:\n  - openapi/edamam-meal-planner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edamam/refs/heads/main/authentication/edamam-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Restaurant
- Food
- Nutrition
- UPC
---
