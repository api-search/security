---
api_key_in:
- query
api_specs:
- filename: edmunds-openapi.yml
  format: yaml
  label: Edmunds Dealership API
  slug: edmunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-openapi.yml
- filename: edmunds-openapi.yml
  format: yaml
  label: Edmunds API
  slug: edmunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Edmunds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edmunds secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edmunds
provider_slug: edmunds
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/edmunds-openapi.yml
  type: apiKey
slug: edmunds-authentication
source_filename: edmunds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/edmunds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/edmunds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/authentication/edmunds-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automobiles
- Cars
- Vehicles
---
