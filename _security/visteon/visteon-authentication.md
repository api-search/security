---
api_key_in:
- header
api_specs:
- filename: visteon-phoenix-openapi.yml
  format: yaml
  label: Visteon Phoenix API
  slug: phoenix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/openapi/visteon-phoenix-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Visteon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Visteon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Visteon
provider_slug: visteon
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Phoenix-API-Key
  sources:
  - openapi/visteon-phoenix-openapi.yml
  type: apiKey
slug: visteon-authentication
source_filename: visteon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/visteon-phoenix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Phoenix-API-Key\n  sources:\n  - openapi/visteon-phoenix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visteon/refs/heads/main/authentication/visteon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Connected Car
- Infotainment
- IoT
- Fortune 500
---
