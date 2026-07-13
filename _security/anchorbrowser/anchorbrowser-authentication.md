---
api_key_in:
- header
api_specs:
- filename: anchorbrowser-openapi.yml
  format: yaml
  label: Anchor Browser API
  slug: anchor-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Anchorbrowser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anchor Browser secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anchor Browser
provider_slug: anchorbrowser
scheme_count: 1
schemes:
- description: API key passed in the header
  in: header
  name: api_key_header
  parameter: anchor-api-key
  sources:
  - openapi/anchorbrowser-openapi.yml
  type: apiKey
slug: anchorbrowser-authentication
source_filename: anchorbrowser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anchorbrowser-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key_header\n  type: apiKey\n  in: header\n  parameter: anchor-api-key\n  description: API key passed in the header\n  sources:\n  - openapi/anchorbrowser-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/authentication/anchorbrowser-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Browser Infrastructure
- AI Agents
- Cloud Browser
- Browser Automation
- Sandbox
- Stealth Browser
- MCP
---
