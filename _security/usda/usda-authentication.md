---
api_key_in:
- query
api_specs:
- filename: fdc_api.html
  format: yaml
  label: USDA FoodData Central API
  slug: usda-fooddata-central-api
  spec_type: OpenAPI
  url: https://fdc.nal.usda.gov/api-spec/fdc_api.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Usda Authentication
name_suffix: Authentication
oauth_flows: []
overview: USDA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: USDA
provider_slug: usda
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/usda-fooddata-central-openapi.yml
  type: apiKey
slug: usda-authentication
source_filename: usda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usda-fooddata-central-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/usda-fooddata-central-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda/refs/heads/main/authentication/usda-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Food Safety
- Nutrition
- Statistics
- Geospatial
- Market News
- Federal Government
---
