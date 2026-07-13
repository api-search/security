---
api_key_in:
- header
api_specs:
- filename: pulse-software-openapi.yml
  format: yaml
  label: Pulse Software
  slug: pulse-software
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pulse Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pulse Software secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pulse Software
provider_slug: pulse-software
scheme_count: 2
schemes:
- in: header
  name: ApiKey
  parameter: x-Api-Key
  sources:
  - openapi/pulse-software-openapi.yml
  type: apiKey
- in: header
  name: BearerJWT
  parameter: Authorisation
  sources:
  - openapi/pulse-software-openapi.yml
  type: apiKey
slug: pulse-software-authentication
source_filename: pulse-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pulse-software-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-Api-Key\n  sources:\n  - openapi/pulse-software-openapi.yml\n- name: BearerJWT\n  type: apiKey\n  in: header\n  parameter: Authorisation\n  sources:\n  - openapi/pulse-software-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/authentication/pulse-software-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Pulse
- Automation
- Developer
---
