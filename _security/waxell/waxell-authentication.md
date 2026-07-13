---
api_key_in:
- header
api_specs:
- filename: waxell-observe-openapi.yml
  format: yaml
  label: Waxell Observe API
  slug: observe
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waxell/refs/heads/main/openapi/waxell-observe-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Waxell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Waxell secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Waxell
provider_slug: waxell
scheme_count: 2
schemes:
- description: Waxell API key issued in the dashboard. Format `wax_sk_...`.
  in: header
  name: WaxKey
  parameter: X-Wax-Key
  sources:
  - openapi/waxell-observe-openapi.yml
  type: apiKey
- bearerFormat: wax_sk
  description: Same `wax_sk_` key passed as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/waxell-observe-openapi.yml
  type: http
slug: waxell-authentication
source_filename: waxell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/waxell-observe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: WaxKey\n  type: apiKey\n  in: header\n  parameter: X-Wax-Key\n  description: Waxell API key issued in the dashboard. Format `wax_sk_...`.\n  sources:\n  - openapi/waxell-observe-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: wax_sk\n  description: Same `wax_sk_` key passed as a Bearer token.\n  sources:\n  - openapi/waxell-observe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waxell/refs/heads/main/authentication/waxell-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Agent Governance
- Observability
- Policy Enforcement
- LLM Telemetry
- Cost Management
- MCP
- Agent Runtime
---
