---
api_key_in:
- query
api_specs:
- filename: nationalize-openapi.json
  format: json
  label: Nationalize.io API
  slug: nationalize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationalize/refs/heads/main/openapi/nationalize-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nationalize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nationalize.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nationalize.io
provider_slug: nationalize
scheme_count: 1
schemes:
- description: API key obtained from https://nationalize.io/login. The same key is shared across all three Demografix services (Genderize, Agify, Nationalize).
  in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/nationalize-openapi.json
  type: apiKey
slug: nationalize-authentication
source_filename: nationalize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nationalize-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key obtained from https://nationalize.io/login. The same key is shared across\n    all three Demografix services (Genderize, Agify, Nationalize).\n  sources:\n  - openapi/nationalize-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationalize/refs/heads/main/authentication/nationalize-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Nationality
- Name Prediction
- Demographics
- Probabilistic Models
- People
---
