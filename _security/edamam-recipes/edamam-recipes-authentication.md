---
api_key_in:
- header
- query
api_specs:
- filename: edamam-recipe-search-v2-openapi.yml
  format: yaml
  label: Edamam Recipe Search API
  slug: edamam-recipe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-recipe-search-v2-openapi.yml
- filename: edamam-nutrition-analysis-v1-openapi.yml
  format: yaml
  label: Edamam Nutrition Analysis API
  slug: edamam-nutrition-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-nutrition-analysis-v1-openapi.yml
- filename: edamam-food-database-v2-openapi.yml
  format: yaml
  label: Edamam Food Database API
  slug: edamam-food-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-food-database-v2-openapi.yml
- filename: edamam-meal-planner-v1-openapi.yml
  format: yaml
  label: Edamam Meal Planner API
  slug: edamam-meal-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-meal-planner-v1-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Edamam Recipes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edamam secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Edamam
provider_slug: edamam-recipes
scheme_count: 4
schemes:
- name: basic
  scheme: basic
  sources:
  - openapi/edamam-meal-planner-v1-openapi.yml
  - openapi/edamam-recipe-search-v2-openapi.yml
  type: http
- description: The application ID, obtained from the account dashboard, https://developer.edamam.com/admin/applications.
  in: query
  name: app_id
  parameter: app_id
  sources:
  - openapi/edamam-recipe-search-v2-openapi.yml
  type: apiKey
- description: The application key, obtained from the account dashboard, https://developer.edamam.com/admin/applications.
  in: query
  name: app_key
  parameter: app_key
  sources:
  - openapi/edamam-recipe-search-v2-openapi.yml
  type: apiKey
- description: ID of the account user. Should be used *only* if the account is configured for active user tracking.
  in: header
  name: Edamam-Account-User
  parameter: Edamam-Account-User
  sources:
  - openapi/edamam-recipe-search-v2-openapi.yml
  type: apiKey
slug: edamam-recipes-authentication
source_filename: edamam-recipes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/edamam-meal-planner-v1-openapi.yml, openapi/edamam-recipe-search-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/edamam-meal-planner-v1-openapi.yml\n  - openapi/edamam-recipe-search-v2-openapi.yml\n- name: app_id\n  type: apiKey\n  in: query\n  parameter: app_id\n  description: The application ID, obtained from the account dashboard, https://developer.edamam.com/admin/applications.\n  sources:\n  - openapi/edamam-recipe-search-v2-openapi.yml\n- name: app_key\n  type: apiKey\n  in: query\n  parameter: app_key\n  description: The application key, obtained from the account dashboard, https://developer.edamam.com/admin/applications.\n  sources:\n  - openapi/edamam-recipe-search-v2-openapi.yml\n- name: Edamam-Account-User\n  type: apiKey\n  in: header\n  parameter: Edamam-Account-User\n  description:\
  \ ID of the account user. Should be used *only* if the account is configured for\n    active user tracking.\n  sources:\n  - openapi/edamam-recipe-search-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/authentication/edamam-recipes-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Food And Drink
- Recipes
- Nutrition
- Diet
- Allergens
- Meal Planning
- Sustainability
- Carbon Footprint
- Public APIs
---
