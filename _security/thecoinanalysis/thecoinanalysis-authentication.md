---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Thecoinanalysis Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Coin Analysis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Coin Analysis
provider_slug: thecoinanalysis
scheme_count: 1
schemes:
- in: header
  name: publicApiKey
  parameter: x-api-key
  sources:
  - openapi/thecoinanalysis-openapi.json
  type: apiKey
slug: thecoinanalysis-authentication
source_filename: thecoinanalysis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: derived\nsource: openapi/thecoinanalysis-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: publicApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/thecoinanalysis-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecoinanalysis/refs/heads/main/authentication/thecoinanalysis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- News
- API
- Data
---
