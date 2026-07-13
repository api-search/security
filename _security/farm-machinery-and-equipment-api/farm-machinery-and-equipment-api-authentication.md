---
api_key_in:
- query
api_specs:
- filename: farm-machinery-and-equipment-api-openapi.yml
  format: yaml
  label: Farm Machinery and Equipment API
  slug: farm-machinery-and-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farm-machinery-and-equipment-api/refs/heads/main/openapi/farm-machinery-and-equipment-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Farm Machinery And Equipment Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farm Machinery and Equipment API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Farm Machinery and Equipment API
provider_slug: farm-machinery-and-equipment-api
scheme_count: 1
schemes:
- in: query
  name: ApiKeyQuery
  parameter: api-key
  sources:
  - openapi/farm-machinery-and-equipment-api-openapi.yml
  type: apiKey
slug: farm-machinery-and-equipment-api-authentication
source_filename: farm-machinery-and-equipment-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/farm-machinery-and-equipment-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/farm-machinery-and-equipment-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farm-machinery-and-equipment-api/refs/heads/main/authentication/farm-machinery-and-equipment-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Equipment
- Farms
- Machinery
---
