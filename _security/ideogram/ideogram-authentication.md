---
api_key_in:
- header
api_specs:
- filename: ideogram-openapi.yml
  format: yaml
  label: Ideogram API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ideogram/refs/heads/main/openapi/ideogram-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ideogram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ideogram secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ideogram
provider_slug: ideogram
scheme_count: 1
schemes:
- description: API key for access control. Use in the header with the name \"Api-Key\"
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/ideogram-openapi.yml
  type: apiKey
slug: ideogram-authentication
source_filename: ideogram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ideogram-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: API key for access control. Use in the header with the name \\\"Api-Key\\\"\n  sources:\n  - openapi/ideogram-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ideogram/refs/heads/main/authentication/ideogram-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Image Generation
- Text
- Realistic
- Editing
---
