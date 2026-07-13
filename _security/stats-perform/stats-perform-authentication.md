---
api_key_in:
- query
api_specs:
- filename: stats-perform-stats-api-openapi.yml
  format: yaml
  label: STATS API
  slug: stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stats-perform/refs/heads/main/openapi/stats-perform-stats-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stats Perform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stats Perform secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stats Perform
provider_slug: stats-perform
scheme_count: 1
schemes:
- description: API key assigned by Stats Perform. An API secret is also assigned for HMAC request signing.
  in: query
  name: statsApiKey
  parameter: api_key
  sources:
  - openapi/stats-perform-stats-api-openapi.yml
  type: apiKey
slug: stats-perform-authentication
source_filename: stats-perform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stats-perform-stats-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: statsApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key assigned by Stats Perform. An API secret is also assigned for HMAC request\n    signing.\n  sources:\n  - openapi/stats-perform-stats-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stats-perform/refs/heads/main/authentication/stats-perform-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports
- Sports Data
- Football
- Baseball
- Basketball
- Hockey
- Soccer
- Golf
- Tennis
- Live Scores
- Statistics
- Sports Analytics
---
