---
api_key_in: []
api_specs:
- filename: workato-developer-api-openapi.yml
  format: yaml
  label: Workato
  slug: workato
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-developer-api-openapi.yml
- filename: workato-event-streams-openapi.yml
  format: yaml
  label: Workato Event Streams Public API
  slug: event-streams-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-event-streams-openapi.yml
- filename: workato-mcp-server-openapi.yml
  format: yaml
  label: Workato MCP Server API
  slug: mcp-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-mcp-server-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workato secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workato
provider_slug: workato
scheme_count: 1
schemes:
- description: 'API client token obtained from the Workato platform. Include as Authorization: Bearer {token}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workato-agent-studio-openapi.yml
  - openapi/workato-developer-api-openapi.yml
  - openapi/workato-event-streams-openapi.yml
  - openapi/workato-mcp-server-openapi.yml
  type: http
slug: workato-authentication
source_filename: workato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workato-agent-studio-openapi.yml, openapi/workato-developer-api-openapi.yml,\n  openapi/workato-event-streams-openapi.yml, openapi/workato-mcp-server-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API client token obtained from the Workato platform. Include as Authorization:\n    Bearer {token}.'\n  sources:\n  - openapi/workato-agent-studio-openapi.yml\n  - openapi/workato-developer-api-openapi.yml\n  - openapi/workato-event-streams-openapi.yml\n  - openapi/workato-mcp-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/authentication/workato-authentication.yml
summary_line: http · 1 scheme
tags:
- Agentic
- API Management
- Automation
- B2B
- Embedded iPaaS
- Enterprise
- Integration
- iPaaS
- Orchestration
- Workflow
---
