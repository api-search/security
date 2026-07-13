---
api_key_in:
- query
api_specs:
- filename: json-spec
  format: yaml
  label: FoodData Central API
  slug: fooddata-central-api
  spec_type: OpenAPI
  url: https://api.nal.usda.gov/fdc/v1/json-spec?api_key=DEMO_KEY
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fooddata Authentication
name_suffix: Authentication
oauth_flows: []
overview: FoodData Central secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FoodData Central
provider_slug: fooddata
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/fooddata-central-api-openapi.json
  type: apiKey
slug: fooddata-authentication
source_filename: fooddata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fooddata-central-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/fooddata-central-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fooddata/refs/heads/main/authentication/fooddata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Food
- Nutrition
- USDA
- Government
- Health
- Diet
- Nutrients
- Public Domain
---
