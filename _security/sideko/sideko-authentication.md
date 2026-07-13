---
api_key_in:
- header
api_specs:
- filename: sideko-openapi.yml
  format: yaml
  label: Sideko API
  slug: sideko-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sideko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sideko secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sideko
provider_slug: sideko
scheme_count: 1
schemes:
- description: Sideko API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: x-sideko-key
  sources:
  - openapi/sideko-openapi.yml
  type: apiKey
slug: sideko-authentication
source_filename: sideko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sideko-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-sideko-key\n  description: Sideko API key for authentication\n  sources:\n  - openapi/sideko-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/authentication/sideko-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CLI
- Documentation
- Mock Servers
- Platform
- SDKs
- API Tooling
- SDK Generation
- MCP Generation
- AI
- Hybrid Codegen
- OpenAPI Linting
---
