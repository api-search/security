---
api_key_in: []
api_specs:
- filename: gumloop-agents-api-openapi.yml
  format: yaml
  label: Gumloop Agents API
  slug: gumloop-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-agents-api-openapi.yml
- filename: gumloop-artifacts-api-openapi.yml
  format: yaml
  label: Gumloop Artifacts API
  slug: gumloop-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-artifacts-api-openapi.yml
- filename: gumloop-brain-api-openapi.yml
  format: yaml
  label: Gumloop Brain API
  slug: gumloop-brain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-brain-api-openapi.yml
- filename: gumloop-chat-completions-api-openapi.yml
  format: yaml
  label: Gumloop Chat completions API
  slug: gumloop-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-chat-completions-api-openapi.yml
- filename: gumloop-data-access-api-openapi.yml
  format: yaml
  label: Gumloop Data Access API
  slug: gumloop-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-data-access-api-openapi.yml
- filename: gumloop-evaluations-api-openapi.yml
  format: yaml
  label: Gumloop Evaluations API
  slug: gumloop-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-evaluations-api-openapi.yml
- filename: gumloop-execution-api-openapi.yml
  format: yaml
  label: Gumloop Execution API
  slug: gumloop-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-execution-api-openapi.yml
- filename: gumloop-file-handling-api-openapi.yml
  format: yaml
  label: Gumloop File Handling API
  slug: gumloop-file-handling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-file-handling-api-openapi.yml
- filename: gumloop-mcp-api-openapi.yml
  format: yaml
  label: Gumloop MCP API
  slug: gumloop-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-mcp-api-openapi.yml
- filename: gumloop-models-api-openapi.yml
  format: yaml
  label: Gumloop Models API
  slug: gumloop-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-models-api-openapi.yml
- filename: gumloop-organization-api-openapi.yml
  format: yaml
  label: Gumloop Organization API
  slug: gumloop-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-organization-api-openapi.yml
- filename: gumloop-sessions-api-openapi.yml
  format: yaml
  label: Gumloop Sessions API
  slug: gumloop-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-sessions-api-openapi.yml
- filename: gumloop-skills-api-openapi.yml
  format: yaml
  label: Gumloop Skills API
  slug: gumloop-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-skills-api-openapi.yml
- filename: gumloop-teams-api-openapi.yml
  format: yaml
  label: Gumloop Teams API
  slug: gumloop-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gumloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gumloop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gumloop
provider_slug: gumloop
scheme_count: 1
schemes:
- description: A personal API key or an [OAuth 2.0](/api-reference/oauth) access token. Personal API keys also require the `x-auth-key` header with your user ID.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gumloop-openapi-original.yml
  type: http
slug: gumloop-authentication
source_filename: gumloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gumloop-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A personal API key or an [OAuth 2.0](/api-reference/oauth) access token. Personal\n    API keys also require the `x-auth-key` header with your user ID.\n  sources:\n  - openapi/gumloop-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/authentication/gumloop-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Workflow-Automation
- Agent Platform
- MCP
- LLM
- No-Code
- Developer Tools
---
