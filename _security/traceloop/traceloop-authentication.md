---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Traceloop REST API
  slug: traceloop-rest-api
  spec_type: OpenAPI
  url: https://www.traceloop.com/docs/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Traceloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Traceloop secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Traceloop
provider_slug: traceloop
scheme_count: 1
schemes:
- description: Type "Bearer" followed by a space and JWT token.
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/traceloop-rest-api-openapi.yml
  type: apiKey
slug: traceloop-authentication
source_filename: traceloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/traceloop-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Type \"Bearer\" followed by a space and JWT token.\n  sources:\n  - openapi/traceloop-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traceloop/refs/heads/main/authentication/traceloop-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- LLM Observability
- OpenTelemetry
- AI Monitoring
- Tracing
- Evaluation
- LLM Gateway
- Prompt Management
- Machine Learning
---
