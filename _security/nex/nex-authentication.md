---
api_key_in:
- header
api_specs:
- filename: nex-ai-lists-api-openapi.yml
  format: yaml
  label: Nex AI Lists API
  slug: nex-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-ai-lists-api-openapi.yml
- filename: nex-compounding-api-openapi.yml
  format: yaml
  label: Nex Compounding API
  slug: nex-compounding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-compounding-api-openapi.yml
- filename: nex-context-api-openapi.yml
  format: yaml
  label: Nex Context API
  slug: nex-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-context-api-openapi.yml
- filename: nex-graph-api-openapi.yml
  format: yaml
  label: Nex Graph API
  slug: nex-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-graph-api-openapi.yml
- filename: nex-insights-api-openapi.yml
  format: yaml
  label: Nex Insights API
  slug: nex-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-insights-api-openapi.yml
- filename: nex-integrations-api-openapi.yml
  format: yaml
  label: Nex Integrations API
  slug: nex-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-integrations-api-openapi.yml
- filename: nex-lists-api-openapi.yml
  format: yaml
  label: Nex Lists API
  slug: nex-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-lists-api-openapi.yml
- filename: nex-notes-api-openapi.yml
  format: yaml
  label: Nex Notes API
  slug: nex-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-notes-api-openapi.yml
- filename: nex-notifications-api-openapi.yml
  format: yaml
  label: Nex Notifications API
  slug: nex-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-notifications-api-openapi.yml
- filename: nex-objects-api-openapi.yml
  format: yaml
  label: Nex Objects API
  slug: nex-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-objects-api-openapi.yml
- filename: nex-records-api-openapi.yml
  format: yaml
  label: Nex Records API
  slug: nex-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-records-api-openapi.yml
- filename: nex-relationships-api-openapi.yml
  format: yaml
  label: Nex Relationships API
  slug: nex-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-relationships-api-openapi.yml
- filename: nex-schema-api-openapi.yml
  format: yaml
  label: Nex Schema API
  slug: nex-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-schema-api-openapi.yml
- filename: nex-search-api-openapi.yml
  format: yaml
  label: Nex Search API
  slug: nex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-search-api-openapi.yml
- filename: nex-tasks-api-openapi.yml
  format: yaml
  label: Nex Tasks API
  slug: nex-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-tasks-api-openapi.yml
- filename: nex-timeline-api-openapi.yml
  format: yaml
  label: Nex Timeline API
  slug: nex-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-timeline-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nex
provider_slug: nex
scheme_count: 1
schemes:
- description: 'API key for authentication (format: "Bearer YOUR_API_KEY")'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/nex-openapi-original.json
  type: apiKey
slug: nex-authentication
source_filename: nex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nex-openapi-original.json\ndocs: https://docs.nex.ai/api-reference/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  format: 'Authorization: Bearer sk-YOUR_API_KEY'\n  scopes_ref: scopes/nex-scopes.yml\n  note: >-\n    API keys are generated from the Nex web UI. Each key carries scopes that\n    gate operations (see scopes/nex-scopes.yml). End-user login to the Nex app\n    itself is brokered by WorkOS AuthKit, but the Developer API is API-key only.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key for authentication (format: \"Bearer YOUR_API_KEY\")'\n  sources:\n  - openapi/nex-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/authentication/nex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Agents
- Knowledge Graph
- Context
- Memory
- MCP
- Workflow-Automation
- Integration
- Developer API
---
