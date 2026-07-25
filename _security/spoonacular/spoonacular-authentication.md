---
api_key_in:
- header
api_specs:
- filename: spoonacular-ingredients-api-openapi.yml
  format: yaml
  label: Spoonacular Ingredients API
  slug: spoonacular-ingredients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-ingredients-api-openapi.yml
- filename: spoonacular-meal-planning-api-openapi.yml
  format: yaml
  label: Spoonacular Meal Planning API
  slug: spoonacular-meal-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-meal-planning-api-openapi.yml
- filename: spoonacular-menu-items-api-openapi.yml
  format: yaml
  label: Spoonacular Menu Items API
  slug: spoonacular-menu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-menu-items-api-openapi.yml
- filename: spoonacular-misc-api-openapi.yml
  format: yaml
  label: Spoonacular Misc API
  slug: spoonacular-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-misc-api-openapi.yml
- filename: spoonacular-products-api-openapi.yml
  format: yaml
  label: Spoonacular Products API
  slug: spoonacular-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-products-api-openapi.yml
- filename: spoonacular-recipes-api-openapi.yml
  format: yaml
  label: Spoonacular Recipes API
  slug: spoonacular-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-recipes-api-openapi.yml
- filename: spoonacular-wine-api-openapi.yml
  format: yaml
  label: Spoonacular Wine API
  slug: spoonacular-wine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/openapi/spoonacular-wine-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spoonacular Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spoonacular secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spoonacular
provider_slug: spoonacular
scheme_count: 1
schemes:
- in: header
  name: apiKeyScheme
  parameter: x-api-key
  sources:
  - openapi/spoonacular-openapi.yml
  type: apiKey
slug: spoonacular-authentication
source_filename: spoonacular-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spoonacular-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyScheme\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/spoonacular-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoonacular/refs/heads/main/authentication/spoonacular-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Food And Drink
- Recipes
- Nutrition
- Meal Planning
- Public APIs
---
