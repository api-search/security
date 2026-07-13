---
api_key_in:
- query
api_specs:
- filename: agify-openapi.json
  format: json
  label: Agify Age Prediction API
  slug: agify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agify/refs/heads/main/openapi/agify-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agify.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agify.io
provider_slug: agify
scheme_count: 1
schemes:
- description: API key obtained from the Agify dashboard. Shared with Genderize.io and Nationalize.io.
  in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/agify-openapi.json
  type: apiKey
slug: agify-authentication
source_filename: agify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agify-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key obtained from the Agify dashboard. Shared with Genderize.io and Nationalize.io.\n  sources:\n  - openapi/agify-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agify/refs/heads/main/authentication/agify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Age Prediction
- Name Analysis
- Demographics
- Statistical API
- Free API
---
