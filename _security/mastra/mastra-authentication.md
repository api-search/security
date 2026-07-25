---
api_key_in: []
api_specs:
- filename: mastra-agents-api-openapi.yml
  format: yaml
  label: Mastra Agents API
  slug: mastra-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-agents-api-openapi.yml
- filename: mastra-conversations-api-openapi.yml
  format: yaml
  label: Mastra Conversations API
  slug: mastra-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-conversations-api-openapi.yml
- filename: mastra-logs-api-openapi.yml
  format: yaml
  label: Mastra Logs API
  slug: mastra-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-logs-api-openapi.yml
- filename: mastra-mcp-api-openapi.yml
  format: yaml
  label: Mastra Mcp API
  slug: mastra-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-mcp-api-openapi.yml
- filename: mastra-memory-api-openapi.yml
  format: yaml
  label: Mastra Memory API
  slug: mastra-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-memory-api-openapi.yml
- filename: mastra-responses-api-openapi.yml
  format: yaml
  label: Mastra Responses API
  slug: mastra-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-responses-api-openapi.yml
- filename: mastra-telemetry-api-openapi.yml
  format: yaml
  label: Mastra Telemetry API
  slug: mastra-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-telemetry-api-openapi.yml
- filename: mastra-tools-api-openapi.yml
  format: yaml
  label: Mastra Tools API
  slug: mastra-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-tools-api-openapi.yml
- filename: mastra-vectors-api-openapi.yml
  format: yaml
  label: Mastra Vectors API
  slug: mastra-vectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-vectors-api-openapi.yml
- filename: mastra-workflows-api-openapi.yml
  format: yaml
  label: Mastra Workflows API
  slug: mastra-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mastra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mastra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mastra
provider_slug: mastra
scheme_count: 1
schemes:
- description: 'Mastra API key passed as `Authorization: Bearer {api_key}`.

    Local dev servers may not require authentication.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mastra-openapi.yml
  type: http
slug: mastra-authentication
source_filename: mastra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mastra-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Mastra API key passed as `Authorization: Bearer {api_key}`.\n    Local dev servers may not require authentication.\n  sources:\n  - openapi/mastra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/authentication/mastra-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- AI
- JavaScript
- RAG
- TypeScript
- Workflows
---
