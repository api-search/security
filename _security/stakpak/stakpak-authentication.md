---
api_key_in:
- cookie
api_specs:
- filename: stakpak-openapi-original.yml
  format: yaml
  label: Stakpak API
  slug: stakpak-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stakpak/refs/heads/main/openapi/stakpak-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stakpak Authentication
name_suffix: Authentication
oauth_flows: []
overview: StakPak secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: StakPak
provider_slug: stakpak
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: Api Key
  scheme: bearer
  sources:
  - openapi/stakpak-openapi-original.yml
  type: http
- in: cookie
  name: cookie
  parameter: .idToken
  sources:
  - openapi/stakpak-openapi-original.yml
  type: apiKey
slug: stakpak-authentication
source_filename: stakpak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/stakpak-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: Api Key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/stakpak-openapi-original.yml\n- name: cookie\n  type: apiKey\n  in: cookie\n  parameter: .idToken\n  sources:\n  - openapi/stakpak-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stakpak/refs/heads/main/authentication/stakpak-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- DevOps
- Infrastructure
- AI Agents
- MCP
- Developer Tools
- CLI
- Cloud
---
