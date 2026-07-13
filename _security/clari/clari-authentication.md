---
api_key_in:
- header
api_specs:
- filename: external_spec
  format: yaml
  label: Clari Revenue API
  slug: clari-revenue-api
  spec_type: OpenAPI
  url: https://developer.clari.com/documentation/external_spec
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clari secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clari
provider_slug: clari
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: apikey
  sources:
  - openapi/clari-revenue-api-openapi.yml
  type: apiKey
slug: clari-authentication
source_filename: clari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clari-revenue-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/clari-revenue-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/authentication/clari-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Revenue Operations
- Forecasting
- Pipeline Management
- Sales Intelligence
- Activity Intelligence
- Deal Insights
- CRM
- Conversation Intelligence
- B2B
- Enterprise
---
