---
api_key_in:
- header
api_specs:
- filename: atomicwork-public-api-openapi.yaml
  format: yaml
  label: Atomicwork Public API
  slug: atomicwork-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-public-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Atomicwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atomicwork secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Atomicwork
provider_slug: atomicwork
scheme_count: 1
schemes:
- description: 'Every request must include a workspace-scoped API key in the X-Api-Key header. Keys are generated from Settings > Integrations > API Keys in the Atomicwork workspace; a key created in one workspace cannot access another.

    '
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/atomicwork-public-api-openapi.yaml
  type: apiKey
slug: atomicwork-authentication
source_filename: atomicwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/atomicwork-public-api-openapi.yaml\ndocs: https://developers.atomicwork.com/api-reference/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >\n    Every request must include a workspace-scoped API key in the X-Api-Key header.\n    Keys are generated from Settings > Integrations > API Keys in the Atomicwork\n    workspace; a key created in one workspace cannot access another.\n  sources:\n  - openapi/atomicwork-public-api-openapi.yaml\nworkspace_scoping:\n  header: X-Workspace-Id\n  description: >\n    Most endpoints are workspace-scoped and require the numeric workspace ID in the\n    X-Workspace-Id header. The workspace ID is visible in Settings > Workspace or\n    returned by GET /api/v1/workspaces.\nnotes: >\n  No OAuth 2.0 / OIDC surface is documented — authentication is API-key only, so\n  no\
  \ scopes/ artifact applies. The same API key authenticates the hosted MCP server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/authentication/atomicwork-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Service Management
- ITSM
- ESM
- IT Service Desk
- Identity Governance
- Asset Management
- AI Agents
- MCP
- Enterprise
---
