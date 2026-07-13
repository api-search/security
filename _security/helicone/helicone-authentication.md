---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: Helicone
  slug: helicone
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: ai-gateway.openapi.json
  format: json
  label: Helicone AI Gateway API
  slug: ai-gateway-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/ai-gateway.openapi.json
- filename: swagger.json
  format: json
  label: Helicone Request API
  slug: request-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Prompt API
  slug: prompt-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Experiment API
  slug: experiment-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Evals API
  slug: evals-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Session API
  slug: session-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone User API
  slug: user-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Webhook API
  slug: webhook-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Model Registry API
  slug: model-registry-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Trace API
  slug: trace-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Dashboard API
  slug: dashboard-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
- filename: swagger.json
  format: json
  label: Helicone Property API
  slug: property-api
  spec_type: OpenAPI
  url: https://docs.helicone.ai/swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Helicone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helicone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Helicone
provider_slug: helicone
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Format: ''Bearer YOUR_API_KEY'''
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/helicone-openapi.yml
  type: apiKey
slug: helicone-authentication
source_filename: helicone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/helicone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Bearer token authentication. Format: ''Bearer YOUR_API_KEY'''\n  sources:\n  - openapi/helicone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helicone/refs/heads/main/authentication/helicone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Gateways
- AI Monitoring
- Gateways
- LLM Observability
- LLM Routing
- Prompt Management
---
