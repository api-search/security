---
api_key_in:
- header
api_specs:
- filename: handwrite-io-openapi.yml
  format: yaml
  label: Handwrite IO API
  slug: handwrite-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/openapi/handwrite-io-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Handwrite Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Handwrite IO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Handwrite IO
provider_slug: handwrite-io
scheme_count: 1
schemes:
- description: API key in the format `live_hw_[key]`
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/handwrite-io-openapi.yml
  type: apiKey
slug: handwrite-io-authentication
source_filename: handwrite-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/handwrite-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key in the format `live_hw_[key]`\n  sources:\n  - openapi/handwrite-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/authentication/handwrite-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Direct Mail
- Handwritten
- Marketing
- Notes
---
