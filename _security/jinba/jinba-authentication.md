---
api_key_in: []
api_specs:
- filename: jinba-toolbox-openapi.yml
  format: yaml
  label: Jinba Toolbox API
  slug: jinba-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-toolbox-openapi.yml
- filename: jinba-flow-openapi.yml
  format: yaml
  label: Jinba Flow External API
  slug: jinba-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-flow-openapi.yml
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
- AI
- Agents
- Workflow Automation
- Enterprise
- MCP
- Low-Code
- Developer Tools
- Tools
- Automation
---
