---
api_key_in:
- header
api_specs:
- filename: radio-cult-openapi.yml
  format: yaml
  label: Radio Cult
  slug: radio-cult
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radio-cult/refs/heads/main/openapi/radio-cult-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Radio Cult Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radio Cult secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Radio Cult
provider_slug: radio-cult
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/radio-cult-openapi.yml
  type: apiKey
slug: radio-cult-authentication
source_filename: radio-cult-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radio-cult-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/radio-cult-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radio-cult/refs/heads/main/authentication/radio-cult-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Radio
- Streaming
- Audio
- Music
- Broadcasting
---
