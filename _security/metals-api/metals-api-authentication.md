---
api_key_in:
- query
api_specs:
- filename: metals-api-openapi.yml
  format: yaml
  label: Metals-API
  slug: metals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-api/refs/heads/main/openapi/metals-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metals Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metals-API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metals-API
provider_slug: metals-api
scheme_count: 1
schemes:
- in: query
  name: accessKey
  parameter: access_key
  sources:
  - openapi/metals-api-openapi.yml
  type: apiKey
slug: metals-api-authentication
source_filename: metals-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metals-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: accessKey\n  type: apiKey\n  in: query\n  parameter: access_key\n  sources:\n  - openapi/metals-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metals-api/refs/heads/main/authentication/metals-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Currency
- Financial Data
- Gold
- Precious Metals
- Silver
---
