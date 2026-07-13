---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Daytona Sandbox API
  slug: sandbox-api
  spec_type: OpenAPI
  url: https://app.daytona.io/api/docs/openapi.json
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Daytona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daytona secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Daytona
provider_slug: daytona
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: API Key access
  name: bearer
  scheme: bearer
  sources:
  - openapi/daytona-openapi.json
  type: http
- name: oauth2
  openIdConnectUrl: http://localhost:3000/.well-known/openid-configuration
  sources:
  - openapi/daytona-openapi.json
  type: openIdConnect
slug: daytona-authentication
source_filename: daytona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/daytona-openapi.json\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: API Key access\n  sources:\n  - openapi/daytona-openapi.json\n- name: oauth2\n  type: openIdConnect\n  openIdConnectUrl: http://localhost:3000/.well-known/openid-configuration\n  sources:\n  - openapi/daytona-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/authentication/daytona-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Sandboxes
- Secure Execution
- AI Agents
- Coding Agents
- Code Interpreter
- Snapshots
- Multi-Region
- HIPAA
- SOC 2
- GDPR
- Python
- TypeScript
- Open Source
- LSP
---
