---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: receptapi-ingredients-api-openapi.yml
  format: yaml
  label: ReceptAPI Ingredients API
  slug: receptapi-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/receptapi/openapi/receptapi-ingredients-api-openapi.yml
- filename: receptapi-recipes-api-openapi.yml
  format: yaml
  label: ReceptAPI Recipes API
  slug: receptapi-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/receptapi/openapi/receptapi-recipes-api-openapi.yml
- filename: receptapi-search-api-openapi.yml
  format: yaml
  label: ReceptAPI Search API
  slug: receptapi-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/receptapi/openapi/receptapi-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ReceptAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReceptAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ReceptAPI
provider_slug: receptapi
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/receptapi-openapi.json
  type: apiKey
slug: receptapi-authentication
source_filename: receptapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/receptapi-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/receptapi-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/receptapi/authentication/receptapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Recipes
- Swedish
- Food
- Data
---
