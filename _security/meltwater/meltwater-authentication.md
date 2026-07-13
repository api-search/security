---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Meltwater API
  slug: meltwater-api
  spec_type: OpenAPI
  url: https://developer.meltwater.com/api-reference/api-reference-overview/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Meltwater Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meltwater secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meltwater
provider_slug: meltwater
scheme_count: 1
schemes:
- in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/meltwater-api-openapi.yaml
  type: apiKey
slug: meltwater-authentication
source_filename: meltwater-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meltwater-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/meltwater-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/authentication/meltwater-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Media Monitoring
- Social Listening
- PR Analytics
- Brand Intelligence
- News API
- Social Analytics
- Media Intelligence
---
