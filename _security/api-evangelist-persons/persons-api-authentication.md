---
api_key_in:
- header
api_specs:
- filename: persons-api-openapi.yml
  format: yaml
  label: Persons API.
  slug: persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-persons/refs/heads/main/openapi/persons-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Persons Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Persons secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Persons
provider_slug: api-evangelist-persons
scheme_count: 1
schemes:
- in: header
  name: apiKeys
  parameter: api-key
  sources:
  - openapi/persons-api-openapi.yml
  type: apiKey
slug: persons-api-authentication
source_filename: persons-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/persons-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeys\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/persons-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-persons/refs/heads/main/authentication/persons-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application Programming Interface
- Persons
---
