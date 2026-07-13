---
api_key_in:
- header
api_specs:
- filename: fashion-ai-openapi.yml
  format: yaml
  label: Fashion AI
  slug: fashion-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fashion-ai/refs/heads/main/openapi/fashion-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fashion Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fashion AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fashion AI
provider_slug: fashion-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/fashion-ai-openapi.yml
  type: apiKey
slug: fashion-ai-authentication
source_filename: fashion-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fashion-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/fashion-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fashion-ai/refs/heads/main/authentication/fashion-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Clothing
- Fashion
---
