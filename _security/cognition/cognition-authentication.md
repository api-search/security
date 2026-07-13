---
api_key_in: []
api_specs:
- filename: cognition-openapi.yml
  format: yaml
  label: Devin API
  slug: devin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cognition Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cognition AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cognition AI
provider_slug: cognition
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cognition-openapi.yml
  type: http
slug: cognition-authentication
source_filename: cognition-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognition-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cognition-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/authentication/cognition-authentication.yml
summary_line: http · 1 scheme
tags:
- Autonomous Agents
- AI Software Engineer
- Coding Agents
- Developer Productivity
- DevOps
- Code Migration
- Code Review
- GitHub Integration
- Enterprise AI
- Agentic Workflows
- IDE
- LLM Applications
---
