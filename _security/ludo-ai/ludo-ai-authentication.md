---
api_key_in:
- header
api_specs:
- filename: ludo-ai-rest-api-openapi.yml
  format: yaml
  label: Ludo.ai REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ludo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ludo.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ludo.ai
provider_slug: ludo-ai
scheme_count: 1
schemes:
- description: 'API key authentication. Pass your API key in the Authentication header with the format: ApiKey YOUR_API_KEY'
  in: header
  name: apiKeyAuth
  parameter: Authentication
  sources:
  - openapi/ludo-ai-rest-api-openapi.yml
  type: apiKey
slug: ludo-ai-authentication
source_filename: ludo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ludo-ai-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: 'API key authentication. Pass your API key in the Authentication header with\n    the format: ApiKey YOUR_API_KEY'\n  sources:\n  - openapi/ludo-ai-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/authentication/ludo-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Asset Generation
- Game Design
- Game Development
---
