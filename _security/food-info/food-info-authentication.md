---
api_key_in: []
api_specs:
- filename: food-info-apiv1-api-openapi.yml
  format: yaml
  label: Food Info API V1 API
  slug: food-info-apiv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/openapi/food-info-apiv1-api-openapi.yml
- filename: food-info-recipesapi-api-openapi.yml
  format: yaml
  label: Food Info Recipes API API
  slug: food-info-recipesapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/openapi/food-info-recipesapi-api-openapi.yml
auth_types: []
description: API key in the X-Api-Key header. HTTPS only, and CORS is disabled — intended for server-to-server use.
kind: authentication
layout: security
method: searched
name: Food Info Authentication
name_suffix: Authentication
oauth_flows: []
overview: Food Info declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Food Info
provider_slug: food-info
scheme_count: 1
schemes:
- id: ApiKey
  in: header
  name: X-Api-Key
  type: apiKey
slug: food-info-authentication
source_filename: food-info-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nstatus: published\nsource: https://api.food-info.org/api/v1/openapi.json\ndescription: API key in the X-Api-Key header. HTTPS only, and CORS is disabled — intended\n  for server-to-server use.\nverified: '2026-08-04'\nschemes:\n- id: ApiKey\n  type: apiKey\n  in: header\n  name: X-Api-Key\nevidence:\n- url: https://api.food-info.org/api/v1/openapi.json\n  status: 200\n  note: securitySchemes read from the published spec\n- url: https://food-info.org/developer\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/authentication/food-info-authentication.yml
summary_line: 1 scheme
tags:
- Nutrition
- Food
- Food Composition
- Nutrients
- Data
- Open Data
- Dietetics
- Recipes
- Health
- Research
---
