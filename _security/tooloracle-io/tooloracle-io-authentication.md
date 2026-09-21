---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tooloracle-io-mcp-platform-openapi.yml
  format: yaml
  label: ToolOracle MCP Platform API
  slug: tooloracle-mcp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-mcp-platform-openapi.yml
- filename: tooloracle-io-x402-v2-openapi.yml
  format: yaml
  label: ToolOracle x402 v2 Compliance, Evidence & Agent-Safety API
  slug: tooloracle-x402-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-x402-v2-openapi.yml
- filename: tooloracle-io-feedoracle-compliance-evidence-openapi.yml
  format: yaml
  label: FeedOracle Compliance Evidence API
  slug: feedoracle-compliance-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Tooloracle Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: FeedOracle Technologies secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FeedOracle Technologies
provider_slug: tooloracle-io
scheme_count: 2
schemes:
- description: Required for v1 data endpoints. Get at /pricing.html
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token from POST /mcp/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml
  type: http
slug: tooloracle-io-authentication
source_filename: tooloracle-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Required for v1 data endpoints. Get at /pricing.html\n  sources:\n  - openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token from POST /mcp/token\n  sources:\n  - openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/authentication/tooloracle-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- MCP
- Agent Infrastructure
- A2A
- x402
- Micropayments
- Compliance
- RegTech
- Blockchain
- Sanctions Screening
- Agent Discovery
- Germany
---
