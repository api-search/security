---
api_key_in:
- header
- query
api_specs:
- filename: apispec
  format: yaml
  label: USDA FoodData Central API
  slug: fooddata-central-api
  spec_type: OpenAPI
  url: https://fdc.nal.usda.gov/portal-data/external/apispec
- filename: usda-ars-ag-data-commons-openapi.yml
  format: yaml
  label: USDA Ag Data Commons CKAN API
  slug: ag-data-commons-ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/openapi/usda-ars-ag-data-commons-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Usda Agricultural Research Service Ars  Authentication
name_suffix: Authentication
oauth_flows: []
overview: USDA Agricultural Research Service (ARS) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: USDA Agricultural Research Service (ARS)
provider_slug: usda-agricultural-research-service-ars-
scheme_count: 2
schemes:
- description: data.gov API key. Register at https://api.data.gov/signup/
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/usda-ars-fooddata-central-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/usda-ars-fooddata-central-openapi.yml
  type: apiKey
slug: usda-agricultural-research-service-ars--authentication
source_filename: usda-agricultural-research-service-ars--authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usda-ars-fooddata-central-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: data.gov API key. Register at https://api.data.gov/signup/\n  sources:\n  - openapi/usda-ars-fooddata-central-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/usda-ars-fooddata-central-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/authentication/usda-agricultural-research-service-ars--authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Open Data
- Research
---
