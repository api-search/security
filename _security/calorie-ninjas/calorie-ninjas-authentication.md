---
api_key_in:
- header
api_specs:
- filename: calorieninjas-openapi.yml
  format: yaml
  label: CalorieNinjas API
  slug: calorieninjas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calorie-ninjas/refs/heads/main/openapi/calorieninjas-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Calorie Ninjas Authentication
name_suffix: Authentication
oauth_flows: []
overview: CalorieNinjas secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CalorieNinjas
provider_slug: calorie-ninjas
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/calorieninjas-openapi.yml
  type: apiKey
slug: calorie-ninjas-authentication
source_filename: calorie-ninjas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/calorieninjas-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/calorieninjas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calorie-ninjas/refs/heads/main/authentication/calorie-ninjas-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Beverages
- Foods
- Image Recognition
- Nutrition
- Recipes
---
