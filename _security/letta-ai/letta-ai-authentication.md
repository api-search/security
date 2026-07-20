---
api_key_in: []
api_specs:
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Agents API
  slug: letta-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Messages API
  slug: letta-ai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Memory Blocks API
  slug: letta-ai-memory-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Archival Memory API
  slug: letta-ai-archival-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Tools API
  slug: letta-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta MCP Servers API
  slug: letta-ai-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Sources and Files API
  slug: letta-ai-sources-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Identities API
  slug: letta-ai-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Multi-Agent Groups API
  slug: letta-ai-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Models and Providers API
  slug: letta-ai-models-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Runs, Jobs and Steps API
  slug: letta-ai-runs-jobs-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Agent Templates API
  slug: letta-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
- filename: letta-ai-openapi.yml
  format: yaml
  label: Letta Chat Completions API
  slug: letta-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Letta Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Letta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Letta
provider_slug: letta-ai
scheme_count: 1
schemes:
- description: 'API key created at https://app.letta.com/api-keys, passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/letta-ai-openapi.yml
  type: http
slug: letta-ai-authentication
source_filename: letta-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/letta-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key created at https://app.letta.com/api-keys, passed as `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/letta-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/authentication/letta-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- LLM
- Memory
- Stateful Agents
- MemGPT
---
