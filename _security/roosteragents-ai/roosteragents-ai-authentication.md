---
anonymous_access: false
api_key_in: []
api_specs:
- filename: roosteragents-ai-agent-readiness-api-openapi.yml
  format: yaml
  label: roosteragents-ai Agent Readiness API
  slug: roosteragents-ai-agent-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-agent-readiness-api-openapi.yml
- filename: roosteragents-ai-gateway-api-openapi.yml
  format: yaml
  label: roosteragents-ai Gateway API
  slug: roosteragents-ai-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-gateway-api-openapi.yml
- filename: roosteragents-ai-mcp-api-openapi.yml
  format: yaml
  label: roosteragents-ai MCP API
  slug: roosteragents-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-mcp-api-openapi.yml
- filename: roosteragents-ai-scan-api-openapi.yml
  format: yaml
  label: roosteragents-ai Scan API
  slug: roosteragents-ai-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-scan-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Roosteragents Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: roosteragents-ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: roosteragents-ai
provider_slug: roosteragents-ai
scheme_count: 1
schemes:
- description: Pay-per-call USDC settlement. 402 challenge, replay with X-PAYMENT.
  name: x402
  scheme: x402
  sources:
  - openapi/roosteragents-ai-openapi.json
  type: http
slug: roosteragents-ai-authentication
source_filename: roosteragents-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/roosteragents-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: x402\n  type: http\n  scheme: x402\n  description: Pay-per-call USDC settlement. 402 challenge, replay with X-PAYMENT.\n  sources:\n  - openapi/roosteragents-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/roosteragents-ai/authentication/roosteragents-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Marketing
- Automation
- SaaS
- Data
---
