---
api_key_in:
- header
api_specs:
- filename: nutritionix-brands-api-openapi.yml
  format: yaml
  label: Nutritionix Brands API
  slug: nutritionix-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-brands-api-openapi.yml
- filename: nutritionix-item-api-openapi.yml
  format: yaml
  label: Nutritionix Item API
  slug: nutritionix-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-item-api-openapi.yml
- filename: nutritionix-natural-language-api-openapi.yml
  format: yaml
  label: Nutritionix Natural Language API
  slug: nutritionix-natural-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-natural-language-api-openapi.yml
- filename: nutritionix-search-api-openapi.yml
  format: yaml
  label: Nutritionix Search API
  slug: nutritionix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nutritionix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nutritionix secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nutritionix
provider_slug: nutritionix
scheme_count: 2
schemes:
- description: Your Nutritionix application identifier.
  in: header
  name: AppId
  parameter: x-app-id
  sources:
  - openapi/nutritionix-track-openapi.yml
  type: apiKey
- description: Your Nutritionix application key.
  in: header
  name: AppKey
  parameter: x-app-key
  sources:
  - openapi/nutritionix-track-openapi.yml
  type: apiKey
slug: nutritionix-authentication
source_filename: nutritionix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nutritionix-track-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppId\n  type: apiKey\n  in: header\n  parameter: x-app-id\n  description: Your Nutritionix application identifier.\n  sources:\n  - openapi/nutritionix-track-openapi.yml\n- name: AppKey\n  type: apiKey\n  in: header\n  parameter: x-app-key\n  description: Your Nutritionix application key.\n  sources:\n  - openapi/nutritionix-track-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/authentication/nutritionix-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Restaurant
- Health
- Nutrition
- Food
- Fitness
- Public APIs
---
