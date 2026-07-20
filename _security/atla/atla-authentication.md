---
api_key_in: []
api_specs:
- filename: atla-insights-openapi.yaml
  format: yaml
  label: Atla Insights API
  slug: atla-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atla/refs/heads/main/openapi/atla-insights-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Atla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atla secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Atla
provider_slug: atla
scheme_count: 1
schemes:
- description: API key authentication using Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/atla-insights-openapi.yaml
  type: http
slug: atla-authentication
source_filename: atla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/atla-insights-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication using Bearer token\n  sources:\n  - openapi/atla-insights-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atla/refs/heads/main/authentication/atla-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SaaS
- Artificial Intelligence
- LLM Evaluation
- AI Agents
- Observability
- Monitoring
- OpenTelemetry
---
