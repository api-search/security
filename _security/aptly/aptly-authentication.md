---
api_key_in:
- header
api_specs:
- filename: aptly-app-api-openapi.yml
  format: yaml
  label: Aptly App API
  slug: aptly-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-app-api-openapi.yml
- filename: aptly-board-api-openapi.yml
  format: yaml
  label: Aptly Board API
  slug: aptly-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-board-api-openapi.yml
- filename: aptly-boards-api-openapi.yml
  format: yaml
  label: Aptly Boards API
  slug: aptly-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-boards-api-openapi.yml
- filename: aptly-cards-api-openapi.yml
  format: yaml
  label: Aptly Cards API
  slug: aptly-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-cards-api-openapi.yml
- filename: aptly-company-api-openapi.yml
  format: yaml
  label: Aptly Company API
  slug: aptly-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-company-api-openapi.yml
- filename: aptly-contacts-api-openapi.yml
  format: yaml
  label: Aptly Contacts API
  slug: aptly-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-contacts-api-openapi.yml
- filename: aptly-email-api-openapi.yml
  format: yaml
  label: Aptly Email API
  slug: aptly-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-email-api-openapi.yml
- filename: aptly-files-api-openapi.yml
  format: yaml
  label: Aptly Files API
  slug: aptly-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-files-api-openapi.yml
- filename: aptly-inboxes-api-openapi.yml
  format: yaml
  label: Aptly Inboxes API
  slug: aptly-inboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-inboxes-api-openapi.yml
- filename: aptly-knowledge-api-openapi.yml
  format: yaml
  label: Aptly Knowledge API
  slug: aptly-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-knowledge-api-openapi.yml
- filename: aptly-routinggroups-api-openapi.yml
  format: yaml
  label: Aptly RoutingGroups API
  slug: aptly-routinggroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-routinggroups-api-openapi.yml
- filename: aptly-schema-api-openapi.yml
  format: yaml
  label: Aptly Schema API
  slug: aptly-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-schema-api-openapi.yml
- filename: aptly-tasks-api-openapi.yml
  format: yaml
  label: Aptly Tasks API
  slug: aptly-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-tasks-api-openapi.yml
- filename: aptly-templates-api-openapi.yml
  format: yaml
  label: Aptly Templates API
  slug: aptly-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-templates-api-openapi.yml
- filename: aptly-users-api-openapi.yml
  format: yaml
  label: Aptly Users API
  slug: aptly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aptly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aptly secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aptly
provider_slug: aptly
scheme_count: 3
schemes:
- in: header
  name: ApiKeyHeader
  parameter: x-token
  sources:
  - openapi/aptly-openapi-original.yml
  type: apiKey
- description: 'Delegate token issued by the platform. Format: `DelegateToken <token>`'
  in: header
  name: DelegateToken
  parameter: Authorization
  sources:
  - openapi/aptly-openapi-original.yml
  type: apiKey
- description: 'Partner token. Format: `Authorization: Bearer <token>`'
  name: PartnerBearer
  scheme: bearer
  sources:
  - openapi/aptly-openapi-original.yml
  type: http
slug: aptly-authentication
source_filename: aptly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/aptly-openapi-original.yml\ndocs: https://docs.getaptly.com/authentication\nnotes: >-\n  Core API uses a static API key passed as the `x-token` header (or `x-token`\n  query parameter) against https://core-api.getaptly.com. Keys are created per\n  company (Board -> Card Sources -> API), work across all boards where the API is\n  enabled, and can carry an optional expiry. Two additional credentials exist:\n  DelegateToken (short-lived scoped JWT for embedded apps / on-behalf-of a user,\n  `Authorization: DelegateToken <token>`) and PartnerBearer (partner token,\n  `Authorization: Bearer <token>`). Delegate scopes are per resource family\n  (boards/inboxes/contacts/files/tasks/email/templates/routing-groups, each\n  read/write). The separate Portal API (app.getaptly.com/api/portal) uses JWT\n  contact-session auth. Errors: 401 missing/invalid/expired key, 403 API not\n  enabled for board, 404 board/card not in company.\n\
  summary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-token\n  sources:\n  - openapi/aptly-openapi-original.yml\n- name: DelegateToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Delegate token issued by the platform. Format: `DelegateToken <token>`'\n  sources:\n  - openapi/aptly-openapi-original.yml\n- name: PartnerBearer\n  type: http\n  scheme: bearer\n  description: 'Partner token. Format: `Authorization: Bearer <token>`'\n  sources:\n  - openapi/aptly-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/authentication/aptly-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Cloud Saas
- Property Management
- Real Estate
- PropTech
- CRM
- Workflow Automation
- AI Agents
- Communications
- MCP
---
