---
api_key_in:
- header
- query
api_specs:
- filename: langflow-base-api-openapi.yml
  format: yaml
  label: Langflow Base API
  slug: langflow-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-base-api-openapi.yml
- filename: langflow-chat-api-openapi.yml
  format: yaml
  label: Langflow Chat API
  slug: langflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-chat-api-openapi.yml
- filename: langflow-files-api-openapi.yml
  format: yaml
  label: Langflow Files API
  slug: langflow-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-files-api-openapi.yml
- filename: langflow-flow-events-api-openapi.yml
  format: yaml
  label: Langflow Flow Events API
  slug: langflow-flow-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-flow-events-api-openapi.yml
- filename: langflow-flows-api-openapi.yml
  format: yaml
  label: Langflow Flows API
  slug: langflow-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-flows-api-openapi.yml
- filename: langflow-health-check-api-openapi.yml
  format: yaml
  label: Langflow Health Check API
  slug: langflow-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-health-check-api-openapi.yml
- filename: langflow-log-api-openapi.yml
  format: yaml
  label: Langflow Log API
  slug: langflow-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-log-api-openapi.yml
- filename: langflow-mcp-api-openapi.yml
  format: yaml
  label: Langflow MCP API
  slug: langflow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-mcp-api-openapi.yml
- filename: langflow-mcp-projects-api-openapi.yml
  format: yaml
  label: Langflow mcp_projects API
  slug: langflow-mcp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-mcp-projects-api-openapi.yml
- filename: langflow-monitor-api-openapi.yml
  format: yaml
  label: Langflow Monitor API
  slug: langflow-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-monitor-api-openapi.yml
- filename: langflow-openai-responses-api-api-openapi.yml
  format: yaml
  label: Langflow OpenAI Responses API API
  slug: langflow-openai-responses-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openai-responses-api-api-openapi.yml
- filename: langflow-projects-api-openapi.yml
  format: yaml
  label: Langflow Projects API
  slug: langflow-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-projects-api-openapi.yml
- filename: langflow-traces-api-openapi.yml
  format: yaml
  label: Langflow Traces API
  slug: langflow-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-traces-api-openapi.yml
- filename: langflow-users-api-openapi.yml
  format: yaml
  label: Langflow Users API
  slug: langflow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-users-api-openapi.yml
- filename: langflow-workflow-api-openapi.yml
  format: yaml
  label: Langflow Workflow API
  slug: langflow-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-workflow-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Langflow Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Langflow secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Langflow
provider_slug: langflow
scheme_count: 3
schemes:
- in: header
  name: API key header
  parameter: x-api-key
  sources:
  - openapi/langflow-openapi.yml
  type: apiKey
- in: query
  name: API key query
  parameter: x-api-key
  sources:
  - openapi/langflow-openapi.yml
  type: apiKey
- flows:
  - flow: password
    scopes: 0
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  sources:
  - openapi/langflow-openapi.yml
  type: oauth2
slug: langflow-authentication
source_filename: langflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - password\nschemes:\n- name: API key header\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/langflow-openapi.yml\n- name: API key query\n  type: apiKey\n  in: query\n  parameter: x-api-key\n  sources:\n  - openapi/langflow-openapi.yml\n- name: OAuth2PasswordBearerCookie\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n    scopes: 0\n  sources:\n  - openapi/langflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/authentication/langflow-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Artificial Intelligence
- Agents
- Workflows
- Low-Code
- Visual Builder
- LangChain
- RAG
- MCP
- Open-Source
- FastAPI
---
