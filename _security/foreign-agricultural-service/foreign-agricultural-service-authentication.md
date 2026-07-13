---
api_key_in:
- header
api_specs:
- filename: foreign-agricultural-service-openapi.yml
  format: yaml
  label: USDA FAS Open Data API
  slug: fas-open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Foreign Agricultural Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Foreign Agricultural Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Foreign Agricultural Service
provider_slug: foreign-agricultural-service
scheme_count: 1
schemes:
- description: API key issued via api.data.gov for the FAS Open Data Services
  in: header
  name: apiKey
  parameter: API_KEY
  sources:
  - openapi/foreign-agricultural-service-openapi.yml
  type: apiKey
slug: foreign-agricultural-service-authentication
source_filename: foreign-agricultural-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/foreign-agricultural-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: API_KEY\n  description: API key issued via api.data.gov for the FAS Open Data Services\n  sources:\n  - openapi/foreign-agricultural-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/authentication/foreign-agricultural-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Federal Government
---
