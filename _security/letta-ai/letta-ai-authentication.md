---
api_key_in: []
api_specs:
- filename: letta-ai-agent-templates-api-openapi.yml
  format: yaml
  label: Letta Agent Templates API
  slug: letta-ai-agent-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-agent-templates-api-openapi.yml
- filename: letta-ai-agents-api-openapi.yml
  format: yaml
  label: Letta Agents API
  slug: letta-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-agents-api-openapi.yml
- filename: letta-ai-archival-memory-api-openapi.yml
  format: yaml
  label: Letta Archival Memory API
  slug: letta-ai-archival-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-archival-memory-api-openapi.yml
- filename: letta-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Letta Chat Completions API
  slug: letta-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-chat-completions-api-openapi.yml
- filename: letta-ai-identities-api-openapi.yml
  format: yaml
  label: Letta Identities API
  slug: letta-ai-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-identities-api-openapi.yml
- filename: letta-ai-mcp-servers-api-openapi.yml
  format: yaml
  label: Letta MCP Servers API
  slug: letta-ai-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-mcp-servers-api-openapi.yml
- filename: letta-ai-memory-blocks-api-openapi.yml
  format: yaml
  label: Letta Memory Blocks API
  slug: letta-ai-memory-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-memory-blocks-api-openapi.yml
- filename: letta-ai-models-and-providers-api-openapi.yml
  format: yaml
  label: Letta Models and Providers API
  slug: letta-ai-models-and-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-models-and-providers-api-openapi.yml
- filename: letta-ai-multi-agent-groups-api-openapi.yml
  format: yaml
  label: Letta Multi-Agent Groups API
  slug: letta-ai-multi-agent-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-multi-agent-groups-api-openapi.yml
- filename: letta-ai-runs-jobs-and-steps-api-openapi.yml
  format: yaml
  label: Letta Runs, Jobs and Steps API
  slug: letta-ai-runs-jobs-and-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-runs-jobs-and-steps-api-openapi.yml
- filename: letta-ai-sources-and-files-api-openapi.yml
  format: yaml
  label: Letta Sources and Files API
  slug: letta-ai-sources-and-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-sources-and-files-api-openapi.yml
- filename: letta-ai-tag-api-openapi.yml
  format: yaml
  label: Letta Tag API
  slug: letta-ai-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-tag-api-openapi.yml
- filename: letta-ai-tools-api-openapi.yml
  format: yaml
  label: Letta Tools API
  slug: letta-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-tools-api-openapi.yml
- filename: letta-ai-voice-api-openapi.yml
  format: yaml
  label: Letta Voice API
  slug: letta-ai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-voice-api-openapi.yml
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
