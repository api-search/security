---
api_key_in:
- header
api_specs:
- filename: radio-mast-openapi.yml
  format: yaml
  label: Radio Mast
  slug: radio-mast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radio-mast/refs/heads/main/openapi/radio-mast-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Radio Mast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radio Mast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Radio Mast
provider_slug: radio-mast
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/radio-mast-openapi.yml
  type: apiKey
slug: radio-mast-authentication
source_filename: radio-mast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/radio-mast-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/radio-mast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radio-mast/refs/heads/main/authentication/radio-mast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Radio
- Streaming
- Analytics
- Audio
- Broadcasting
---
