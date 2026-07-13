---
api_key_in:
- query
api_specs:
- filename: national-agricultural-library-openapi.json
  format: json
  label: USDA FoodData Central API
  slug: fooddata-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-agricultural-library/main/openapi/national-agricultural-library-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Agricultural Library Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Agricultural Library secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Agricultural Library
provider_slug: national-agricultural-library
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/national-agricultural-library-openapi.json
  type: apiKey
slug: national-agricultural-library-authentication
source_filename: national-agricultural-library-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-agricultural-library-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/national-agricultural-library-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-agricultural-library/refs/heads/main/authentication/national-agricultural-library-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Federal Government
- Library
- Food
- Nutrition
---
