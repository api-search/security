---
api_key_in:
- query
api_specs:
- filename: azumio-food-recognition-openapi.yml
  format: yaml
  label: Calorie Mama Food Recognition API
  slug: calorie-mama-food-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azumio/refs/heads/main/openapi/azumio-food-recognition-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Azumio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azumio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azumio
provider_slug: azumio
scheme_count: 1
schemes:
- description: 3scale application API key passed as the query parameter user_key on every request. Keys are issued from the Calorie Mama developer portal after sign-up and are tied to a usage plan.
  in: query
  name: user_key
  parameter: user_key
  sources:
  - openapi/azumio-food-recognition-openapi.yml
  type: apiKey
slug: azumio-authentication
source_filename: azumio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://dev.caloriemama.ai/docs\ndocs: https://dev.caloriemama.ai/docs\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: user_key\n    type: apiKey\n    in: query\n    parameter: user_key\n    description: >-\n      3scale application API key passed as the query parameter user_key on every\n      request. Keys are issued from the Calorie Mama developer portal after\n      sign-up and are tied to a usage plan.\n    sources: [openapi/azumio-food-recognition-openapi.yml]\nnotes:\n  - The API is fronted by a 3scale (APIcast) gateway; auth is application-key\n    only. No OAuth, no bearer tokens, no scopes are documented.\n  - Sign up for a key at https://dev.caloriemama.ai/signup ; manage at\n    https://dev.caloriemama.ai/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azumio/refs/heads/main/authentication/azumio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Health
- Digital Health
- Nutrition
- Food Recognition
- Machine Learning
- Artificial Intelligence
- Fitness
- Diabetes
- API
---
