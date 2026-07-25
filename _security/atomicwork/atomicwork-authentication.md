---
api_key_in:
- header
api_specs:
- filename: atomicwork-accessmanagement-api-openapi.yml
  format: yaml
  label: Atomicwork accessManagement API
  slug: atomicwork-accessmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-accessmanagement-api-openapi.yml
- filename: atomicwork-agentgroups-api-openapi.yml
  format: yaml
  label: Atomicwork agentGroups API
  slug: atomicwork-agentgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-agentgroups-api-openapi.yml
- filename: atomicwork-assets-api-openapi.yml
  format: yaml
  label: Atomicwork assets API
  slug: atomicwork-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-assets-api-openapi.yml
- filename: atomicwork-auditlogs-api-openapi.yml
  format: yaml
  label: Atomicwork auditLogs API
  slug: atomicwork-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-auditlogs-api-openapi.yml
- filename: atomicwork-businesshourconfig-api-openapi.yml
  format: yaml
  label: Atomicwork businessHourConfig API
  slug: atomicwork-businesshourconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-businesshourconfig-api-openapi.yml
- filename: atomicwork-changemanagement-api-openapi.yml
  format: yaml
  label: Atomicwork changeManagement API
  slug: atomicwork-changemanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-changemanagement-api-openapi.yml
- filename: atomicwork-customobjects-api-openapi.yml
  format: yaml
  label: Atomicwork customObjects API
  slug: atomicwork-customobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-customobjects-api-openapi.yml
- filename: atomicwork-entities-api-openapi.yml
  format: yaml
  label: Atomicwork entities API
  slug: atomicwork-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-entities-api-openapi.yml
- filename: atomicwork-forms-api-openapi.yml
  format: yaml
  label: Atomicwork forms API
  slug: atomicwork-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-forms-api-openapi.yml
- filename: atomicwork-problems-api-openapi.yml
  format: yaml
  label: Atomicwork problems API
  slug: atomicwork-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-problems-api-openapi.yml
- filename: atomicwork-requests-api-openapi.yml
  format: yaml
  label: Atomicwork requests API
  slug: atomicwork-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-requests-api-openapi.yml
- filename: atomicwork-servicecatalog-api-openapi.yml
  format: yaml
  label: Atomicwork serviceCatalog API
  slug: atomicwork-servicecatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-servicecatalog-api-openapi.yml
- filename: atomicwork-tags-api-openapi.yml
  format: yaml
  label: Atomicwork tags API
  slug: atomicwork-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-tags-api-openapi.yml
- filename: atomicwork-users-api-openapi.yml
  format: yaml
  label: Atomicwork users API
  slug: atomicwork-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-users-api-openapi.yml
- filename: atomicwork-workflows-api-openapi.yml
  format: yaml
  label: Atomicwork workflows API
  slug: atomicwork-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-workflows-api-openapi.yml
- filename: atomicwork-workspaces-api-openapi.yml
  format: yaml
  label: Atomicwork workspaces API
  slug: atomicwork-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-workspaces-api-openapi.yml
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
