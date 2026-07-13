---
api_key_in:
- query
api_specs:
- filename: cities-database-api-openapi.yml
  format: yaml
  label: AirLabs Cities API
  slug: airlabs-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cities-database-api/refs/heads/main/openapi/cities-database-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cities Database Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cities Database API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cities Database API
provider_slug: cities-database-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/cities-database-api-openapi.yml
  type: apiKey
slug: cities-database-api-authentication
source_filename: cities-database-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cities-database-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/cities-database-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cities-database-api/refs/heads/main/authentication/cities-database-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cities
- Data
- Geography
- Locations
- Reference Data
- Travel
---
