---
api_key_in: []
api_specs:
- filename: agent-diff-sandbox-openapi.yml
  format: yaml
  label: Agent Diff Sandbox API
  slug: agent-diff-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/openapi/agent-diff-sandbox-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agent Diff Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Diff secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agent Diff
provider_slug: agent-diff
scheme_count: 1
schemes:
- description: Bearer token authentication for Agent Diff API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agent-diff-sandbox-openapi.yml
  type: http
slug: agent-diff-authentication
source_filename: agent-diff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agent-diff-sandbox-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for Agent Diff API.\n  sources:\n  - openapi/agent-diff-sandbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/authentication/agent-diff-authentication.yml
summary_line: http · 1 scheme
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
---
