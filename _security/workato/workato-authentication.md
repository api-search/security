---
api_key_in: []
api_specs:
- filename: workato-data-tables-api-openapi.yml
  format: yaml
  label: Workato Data Tables API
  slug: workato-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-data-tables-api-openapi.yml
- filename: workato-genies-api-openapi.yml
  format: yaml
  label: Workato Genies API
  slug: workato-genies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-genies-api-openapi.yml
- filename: workato-knowledge-bases-api-openapi.yml
  format: yaml
  label: Workato Knowledge Bases API
  slug: workato-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-knowledge-bases-api-openapi.yml
- filename: workato-mcp-servers-api-openapi.yml
  format: yaml
  label: Workato MCP Servers API
  slug: workato-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-mcp-servers-api-openapi.yml
- filename: workato-messages-api-openapi.yml
  format: yaml
  label: Workato Messages API
  slug: workato-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-messages-api-openapi.yml
- filename: workato-policies-api-openapi.yml
  format: yaml
  label: Workato Policies API
  slug: workato-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-policies-api-openapi.yml
- filename: workato-recipes-api-openapi.yml
  format: yaml
  label: Workato Recipes API
  slug: workato-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-recipes-api-openapi.yml
- filename: workato-skills-api-openapi.yml
  format: yaml
  label: Workato Skills API
  slug: workato-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-skills-api-openapi.yml
- filename: workato-tools-api-openapi.yml
  format: yaml
  label: Workato Tools API
  slug: workato-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-tools-api-openapi.yml
- filename: workato-user-groups-api-openapi.yml
  format: yaml
  label: Workato User Groups API
  slug: workato-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-user-groups-api-openapi.yml
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
- Workflows
---
