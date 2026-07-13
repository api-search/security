---
api_key_in: []
api_specs:
- filename: monoscope-platform-openapi.yml
  format: yaml
  label: Monoscope Platform API
  slug: monoscope-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitoolkit/refs/heads/main/openapi/monoscope-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apitoolkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIToolkit (Monoscope) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIToolkit (Monoscope)
provider_slug: apitoolkit
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Project-scoped Bearer API key. Create via Settings > API Keys in the

    Monoscope dashboard; keys are shown once and are scoped to a single

    project.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/monoscope-platform-openapi.yml
  type: http
slug: apitoolkit-authentication
source_filename: apitoolkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monoscope-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: |-\n    Project-scoped Bearer API key. Create via Settings > API Keys in the\n    Monoscope dashboard; keys are shown once and are scoped to a single\n    project.\n  sources:\n  - openapi/monoscope-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apitoolkit/refs/heads/main/authentication/apitoolkit-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Observability
- API Analytics
- API Catalog
- API Management
- API Monitoring
- API Testing
- Breaking Change Detection
- CLI
- Debugging
- Error Tracking
- LLM Observability
- Logs and Traces
- MCP Server
- Metrics
- Monitors
- Observability
- OpenTelemetry
- Platform
- Session Replay
---
