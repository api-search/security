---
api_key_in:
- query
api_specs:
- filename: prevedere-openapi-original.json
  format: json
  label: Board Foresight API (V1)
  slug: board-foresight-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prevedere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prevedere secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prevedere
provider_slug: prevedere
scheme_count: 1
schemes:
- in: query
  name: api key
  parameter: ApiKey
  sources:
  - openapi/prevedere-openapi-original.json
  type: apiKey
slug: prevedere-authentication
source_filename: prevedere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/prevedere-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api key\n  type: apiKey\n  in: query\n  parameter: ApiKey\n  sources:\n  - openapi/prevedere-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/authentication/prevedere-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Economic Forecasting
- Predictive Analytics
- Demand Planning
- Financial Planning
- Macroeconomic Data
- Indicators
- Time Series
- Data Integration
- Machine Learning
---
