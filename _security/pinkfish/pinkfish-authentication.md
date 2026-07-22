---
api_key_in:
- header
api_specs:
- filename: pinkfish-triggers-openapi.yml
  format: yaml
  label: Pinkfish Triggers API
  slug: pinkfish-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinkfish/refs/heads/main/openapi/pinkfish-triggers-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pinkfish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinkfish secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pinkfish
provider_slug: pinkfish
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/pinkfish-triggers-openapi.yml
  type: apiKey
slug: pinkfish-authentication
source_filename: pinkfish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pinkfish-triggers-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/pinkfish-triggers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinkfish/refs/heads/main/authentication/pinkfish-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic Workflows
- Automation
- Orchestration
- Model Context Protocol
- Integrations
- Enterprise
- No-Code
---
