---
api_key_in: []
api_specs:
- filename: warp-oz-agent-api-openapi.yml
  format: yaml
  label: Warp Oz Agent API
  slug: oz-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warp/refs/heads/main/openapi/warp-oz-agent-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Warp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Warp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Warp
provider_slug: warp
scheme_count: 1
schemes:
- description: Authentication via a Warp API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/warp-oz-agent-api-openapi.yml
  type: http
slug: warp-authentication
source_filename: warp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warp-oz-agent-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Authentication via a Warp API key.\n  sources:\n  - openapi/warp-oz-agent-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warp/refs/heads/main/authentication/warp-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Terminal
- AI Agents
- Cloud Agents
- Agentic Development
---
