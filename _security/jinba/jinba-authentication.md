---
api_key_in: []
api_specs:
- filename: jinba-api-keys-api-openapi.yml
  format: yaml
  label: Jinba API Keys API
  slug: jinba-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-api-keys-api-openapi.yml
- filename: jinba-credits-api-openapi.yml
  format: yaml
  label: Jinba Credits API
  slug: jinba-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-credits-api-openapi.yml
- filename: jinba-execution-api-openapi.yml
  format: yaml
  label: Jinba Execution API
  slug: jinba-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-execution-api-openapi.yml
- filename: jinba-explore-api-openapi.yml
  format: yaml
  label: Jinba Explore API
  slug: jinba-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-explore-api-openapi.yml
- filename: jinba-flows-api-openapi.yml
  format: yaml
  label: Jinba Flows API
  slug: jinba-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-flows-api-openapi.yml
- filename: jinba-mcp-api-openapi.yml
  format: yaml
  label: Jinba MCP API
  slug: jinba-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-mcp-api-openapi.yml
- filename: jinba-members-api-openapi.yml
  format: yaml
  label: Jinba Members API
  slug: jinba-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-members-api-openapi.yml
- filename: jinba-organizations-api-openapi.yml
  format: yaml
  label: Jinba Organizations API
  slug: jinba-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-organizations-api-openapi.yml
- filename: jinba-public-api-openapi.yml
  format: yaml
  label: Jinba Public API
  slug: jinba-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-public-api-openapi.yml
- filename: jinba-runs-api-openapi.yml
  format: yaml
  label: Jinba Runs API
  slug: jinba-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-runs-api-openapi.yml
- filename: jinba-tools-api-openapi.yml
  format: yaml
  label: Jinba Tools API
  slug: jinba-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-tools-api-openapi.yml
- filename: jinba-toolsets-api-openapi.yml
  format: yaml
  label: Jinba ToolSets API
  slug: jinba-toolsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-toolsets-api-openapi.yml
- filename: jinba-versions-api-openapi.yml
  format: yaml
  label: Jinba Versions API
  slug: jinba-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-versions-api-openapi.yml
- filename: jinba-webhooks-api-openapi.yml
  format: yaml
  label: Jinba Webhooks API
  slug: jinba-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-webhooks-api-openapi.yml
auth_types:
- http
description: 'Jinba authenticates programmatic access with Bearer API keys. Jinba Toolbox supports two methods: session-based auth (Better Auth session cookies) for the admin web console, and organization-scoped API keys (jtb_ prefix) passed as a Bearer token for the SDK, AI agents, and external integrations. Jinba Flow''s External API uses a per-flow Bearer API key that is auto-generated when a workflow is published. There is no OAuth2 authorization flow and no documented scope surface; access is governed by organization-level RBAC (Owner/Admin/ Member) and PostgreSQL row-level security tenant isolation.'
kind: authentication
layout: security
method: searched
name: Jinba Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jinba secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jinba
provider_slug: jinba
scheme_count: 3
schemes:
- expiration: none by default (valid until manually deleted)
  header: 'Authorization: Bearer [example key]'
  key_prefix: jtb_
  name: toolbox-api-key
  notes: Keys are scoped to a single organization, track their issuer, record a last-used timestamp, and creation/deletion is audit-logged.
  scheme: bearer
  scope: organization
  sources:
  - openapi/jinba-toolbox-openapi.yml
  - https://docs.jinba.io/en/pages/toolbox/advanced/security
  type: http
- mechanism: Better Auth session cookies
  name: toolbox-session
  scope: web console (human users)
  sources:
  - https://docs.jinba.io/en/pages/toolbox/advanced/security
  type: session
- header: 'Authorization: Bearer [example key]'
  name: flow-api-key
  notes: Auto-generated on publish; regenerating invalidates the old key immediately.
  scheme: bearer
  scope: per published flow
  sources:
  - openapi/jinba-flow-openapi.yml
  - https://docs.jinba.io/en/pages/basics/api
  type: http
slug: jinba-authentication
source_filename: jinba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://docs.jinba.io/en/pages/toolbox/advanced/security and\n  https://docs.jinba.io/en/pages/toolbox/developer/api and\n  https://docs.jinba.io/en/pages/basics/api\ndocs: https://docs.jinba.io/en/pages/toolbox/advanced/security\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_prefix: jtb_\n  oauth2_flows: []\ndescription: >-\n  Jinba authenticates programmatic access with Bearer API keys. Jinba Toolbox\n  supports two methods: session-based auth (Better Auth session cookies) for the\n  admin web console, and organization-scoped API keys (jtb_ prefix) passed as a\n  Bearer token for the SDK, AI agents, and external integrations. Jinba Flow's\n  External API uses a per-flow Bearer API key that is auto-generated when a\n  workflow is published. There is no OAuth2 authorization flow and no documented\n  scope surface; access is governed by organization-level RBAC (Owner/Admin/\n  Member) and PostgreSQL\
  \ row-level security tenant isolation.\nschemes:\n- name: toolbox-api-key\n  type: http\n  scheme: bearer\n  key_prefix: jtb_\n  scope: organization\n  header: 'Authorization: Bearer [example key]'\n  expiration: none by default (valid until manually deleted)\n  notes: >-\n    Keys are scoped to a single organization, track their issuer, record a\n    last-used timestamp, and creation/deletion is audit-logged.\n  sources:\n  - openapi/jinba-toolbox-openapi.yml\n  - https://docs.jinba.io/en/pages/toolbox/advanced/security\n- name: toolbox-session\n  type: session\n  mechanism: Better Auth session cookies\n  scope: web console (human users)\n  sources:\n  - https://docs.jinba.io/en/pages/toolbox/advanced/security\n- name: flow-api-key\n  type: http\n  scheme: bearer\n  scope: per published flow\n  header: 'Authorization: Bearer [example key]'\n  notes: Auto-generated on publish; regenerating invalidates the old key immediately.\n  sources:\n  - openapi/jinba-flow-openapi.yml\n  - https://docs.jinba.io/en/pages/basics/api\n\
  rbac:\n  roles: [Owner, Admin, Member, super_admin]\n  isolation: organization-based; PostgreSQL Row Level Security enforces tenant isolation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/authentication/jinba-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- Workflow-Automation
- Enterprise
- MCP
- Low-Code
- Developer Tools
- Tools
- Automation
---
