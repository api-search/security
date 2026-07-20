---
api_key_in:
- header
api_specs:
- filename: ardent-openapi-original.json
  format: json
  label: Ardent API
  slug: ardent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ardent/refs/heads/main/openapi/ardent-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ardent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ardent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ardent
provider_slug: ardent
scheme_count: 1
schemes:
- description: 'Ardent API key or a dashboard session token, sent as an Authorization: Bearer header. API keys are minted in the dashboard (Settings > API keys) or via the API-keys endpoints, and carry the prefix sk-ard_live_ (production) or sk-ard_test_ (test).'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ardent-openapi-original.json
  type: http
slug: ardent-authentication
source_filename: ardent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/ardent-openapi-original.json\ndocs: https://docs.tryardent.com/api/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  key_prefixes:\n  - sk-ard_live_\n  - sk-ard_test_\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Ardent API key or a dashboard session token, sent as an Authorization: Bearer header.\n    API keys are minted in the dashboard (Settings > API keys) or via the API-keys endpoints,\n    and carry the prefix sk-ard_live_ (production) or sk-ard_test_ (test).\n  in: header\n  header: Authorization\n  sources:\n  - openapi/ardent-openapi-original.json\n# Role-based access control (assigned per API key / member, not OAuth scopes)\nroles:\n- id: role_org_viewer\n  description: Read-only access for automation and reporting.\n- id: role_org_member\n  description: Create and modify resources such as branches and connectors.\n- id: role_org_admin\n  description:\
  \ Team and API-key management.\n- id: role_org_owner\n  description: Complete organization control.\nroles_source: https://docs.tryardent.com/api/authentication\nroles_endpoint: GET /v1/orgs/{org_id}/roles\nnotes: >-\n  No OAuth 2.0 / OIDC flows are declared; access is bearer-key based with server-side RBAC roles,\n  so there is no OAuth scope surface (scopes/ intentionally omitted).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ardent/refs/heads/main/authentication/ardent-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Database
- PostgreSQL
- Database Branching
- Developer Tools
- Sandbox
- AI Agents
- CI/CD
- Data Infrastructure
- Testing
---
