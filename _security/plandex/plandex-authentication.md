---
api_key_in: []
api_specs:
- filename: plandex-server-openapi.yml
  format: yaml
  label: Plandex Server API
  slug: plandex-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plandex/main/openapi/plandex-server-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Plandex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plandex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plandex
provider_slug: plandex
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token issued by the Plandex server on sign-in. Used by the CLI/REPL for all authenticated API calls.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/plandex-server-openapi.yml
  type: http
slug: plandex-authentication
source_filename: plandex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plandex-server-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token issued by the Plandex server on sign-in. Used by the CLI/REPL for\n    all authenticated API calls.\n  sources:\n  - openapi/plandex-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plandex/refs/heads/main/authentication/plandex-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- AI Coding Agent
- Developer Tools
- Open Source
- CLI
- Terminal
- LLM
- Coding Assistant
- Agents
- Go
- Context Management
- Plans
- Self-Hosted
- REST
---
