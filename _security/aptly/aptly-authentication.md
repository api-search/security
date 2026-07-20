---
api_key_in:
- header
api_specs:
- filename: aptly-openapi-original.yml
  format: yaml
  label: Aptly Core API
  slug: aptly-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptly/refs/heads/main/openapi/aptly-openapi-original.yml
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
