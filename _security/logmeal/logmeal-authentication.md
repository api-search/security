---
api_key_in: []
api_specs:
- filename: logmeal-food-recognition-api-openapi.yml
  format: yaml
  label: LogMeal Food Recognition API
  slug: food-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logmeal/refs/heads/main/openapi/logmeal-food-recognition-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Logmeal Authentication
name_suffix: Authentication
oauth_flows: []
overview: LogMeal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LogMeal
provider_slug: logmeal
scheme_count: 1
schemes:
- description: User access token issued by LogMeal.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/logmeal-food-recognition-api-openapi.yml
  type: http
slug: logmeal-authentication
source_filename: logmeal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/logmeal-food-recognition-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: User access token issued by LogMeal.\n  sources:\n  - openapi/logmeal-food-recognition-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logmeal/refs/heads/main/authentication/logmeal-authentication.yml
summary_line: http · 1 scheme
tags:
- Computer Vision
- Food
- Image Recognition
- Nutrition
- Semantic Tagging
---
