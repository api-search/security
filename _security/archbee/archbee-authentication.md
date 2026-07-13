---
api_key_in:
- header
api_specs:
- filename: archbee-api.yaml
  format: yaml
  label: Archbee API
  slug: archbee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Archbee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archbee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Archbee
provider_slug: archbee
scheme_count: 1
schemes:
- description: Archbee API key from the workspace settings
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/archbee-api.yaml
  type: apiKey
slug: archbee-authentication
source_filename: archbee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/archbee-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Archbee API key from the workspace settings\n  sources:\n  - openapi/archbee-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/authentication/archbee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
---
