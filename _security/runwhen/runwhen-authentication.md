---
api_key_in: []
api_specs:
- filename: runwhen-papi-openapi-original.json
  format: json
  label: RunWhen Platform API (PAPI)
  slug: runwhen-platform-api-papi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwhen/refs/heads/main/openapi/runwhen-papi-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runwhen Authentication
name_suffix: Authentication
oauth_flows: []
overview: RunWhen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RunWhen
provider_slug: runwhen
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT access token from /api/v3/token/ or Auth0 login
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/runwhen-papi-openapi-original.json
  type: http
slug: runwhen-authentication
source_filename: runwhen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/runwhen-papi-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token from /api/v3/token/ or Auth0 login\n  sources:\n  - openapi/runwhen-papi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runwhen/refs/heads/main/authentication/runwhen-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AIOps
- SRE
- DevOps
- Observability
- Incident Response
- AI Agents
- Kubernetes
- Automation
- MCP
---
