---
api_key_in:
- query
api_specs:
- filename: yaml-spec
  format: yaml
  label: USDA FoodData Central API
  slug: usda-fooddata-central-api
  spec_type: OpenAPI
  url: https://api.nal.usda.gov/fdc/v1/yaml-spec?api_key=DEMO_KEY
- filename: usda-nass-quickstats-openapi.yml
  format: yaml
  label: USDA NASS Quick Stats API
  slug: usda-nass-quickstats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/usda-nass-quickstats-openapi.yml
- filename: usda-ers-arms-openapi.yml
  format: yaml
  label: USDA ERS ARMS Data API
  slug: usda-ers-arms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/usda-ers-arms-openapi.yml
- filename: usda-nrcs-awdb-openapi.yml
  format: yaml
  label: USDA NRCS AWDB Water and Climate REST API
  slug: usda-nrcs-awdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/usda-nrcs-awdb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: United States Department Of Agriculture Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States Department of Agriculture secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: United States Department of Agriculture
provider_slug: united-states-department-of-agriculture
scheme_count: 2
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/usda-ers-arms-openapi.yml
  - openapi/usda-fooddata-central-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/usda-nass-quickstats-openapi.yml
  type: apiKey
slug: united-states-department-of-agriculture-authentication
source_filename: united-states-department-of-agriculture-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usda-ers-arms-openapi.yml, openapi/usda-fooddata-central-openapi.yml, openapi/usda-nass-quickstats-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/usda-ers-arms-openapi.yml\n  - openapi/usda-fooddata-central-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/usda-nass-quickstats-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/authentication/united-states-department-of-agriculture-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Rural Development
- Climate
---
