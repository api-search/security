---
api_key_in: []
api_specs:
- filename: fatsecret-platform-openapi.yml
  format: yaml
  label: FatSecret Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-platform-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fatsecret Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FatSecret secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FatSecret
provider_slug: fatsecret
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://oauth.fatsecret.com/connect/token
  name: oauth2
  sources:
  - openapi/fatsecret-platform-openapi.yml
  type: oauth2
- description: OAuth 1.0a request signing
  name: oauth1
  scheme: oauth
  sources:
  - openapi/fatsecret-platform-openapi.yml
  type: http
slug: fatsecret-authentication
source_filename: fatsecret-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fatsecret-platform-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.fatsecret.com/connect/token\n    scopes: 2\n  sources:\n  - openapi/fatsecret-platform-openapi.yml\n- name: oauth1\n  type: http\n  scheme: oauth\n  description: OAuth 1.0a request signing\n  sources:\n  - openapi/fatsecret-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/authentication/fatsecret-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Barcode Scanning
- Calories
- Diets
- Exercise
- Fitness
- Food Diary
- Health
- Macronutrients
- Nutrition
- Recipes
- Weight Tracking
---
