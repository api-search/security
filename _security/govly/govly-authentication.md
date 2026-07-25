---
api_key_in:
- header
api_specs:
- filename: govly-awards-api-openapi.yml
  format: yaml
  label: Govly Awards API
  slug: govly-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-awards-api-openapi.yml
- filename: govly-documents-api-openapi.yml
  format: yaml
  label: Govly Documents API
  slug: govly-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-documents-api-openapi.yml
- filename: govly-follows-api-openapi.yml
  format: yaml
  label: Govly Follows API
  slug: govly-follows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-follows-api-openapi.yml
- filename: govly-inbox-api-openapi.yml
  format: yaml
  label: Govly Inbox API
  slug: govly-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-inbox-api-openapi.yml
- filename: govly-opportunities-api-openapi.yml
  format: yaml
  label: Govly Opportunities API
  slug: govly-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-opportunities-api-openapi.yml
- filename: govly-quote-submissions-api-openapi.yml
  format: yaml
  label: Govly Quote Submissions API
  slug: govly-quote-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-quote-submissions-api-openapi.yml
- filename: govly-saved-searches-api-openapi.yml
  format: yaml
  label: Govly Saved Searches API
  slug: govly-saved-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-saved-searches-api-openapi.yml
- filename: govly-workspace-attachments-api-openapi.yml
  format: yaml
  label: Govly Workspace Attachments API
  slug: govly-workspace-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-workspace-attachments-api-openapi.yml
- filename: govly-workspace-comments-api-openapi.yml
  format: yaml
  label: Govly Workspace Comments API
  slug: govly-workspace-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-workspace-comments-api-openapi.yml
- filename: govly-workspace-members-api-openapi.yml
  format: yaml
  label: Govly Workspace Members API
  slug: govly-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-workspace-members-api-openapi.yml
- filename: govly-workspaces-api-openapi.yml
  format: yaml
  label: Govly Workspaces API
  slug: govly-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Govly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Govly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Govly
provider_slug: govly
scheme_count: 2
schemes:
- bearerFormat: API key
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/govly-tools-v1-openapi-original.yml
  type: http
- in: header
  name: headerApiKey
  parameter: X-API-KEY
  sources:
  - openapi/govly-tools-v1-openapi-original.yml
  type: apiKey
slug: govly-authentication
source_filename: govly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/govly-tools-v1-openapi-original.yml\ndocs: https://docs.govly.com/getting-started/introduction\nnotes: >-\n  Govly authenticates with a personal API key generated from Settings -> API ->\n  API Keys in the Govly app. Keys carry a \"gk_\" prefix and are shown only once.\n  The key may be sent either as an HTTP bearer token (Authorization: Bearer\n  gk_...) or in the X-API-KEY header. The API only responds over HTTPS and returns\n  JSON. The hosted MCP server additionally supports an OAuth sign-in flow (managed\n  under Settings -> API -> Connected Apps) as an alternative to a personal key.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  sources:\n  - openapi/govly-tools-v1-openapi-original.yml\n- name: headerApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/govly-tools-v1-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/authentication/govly-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Government
- Public Sector
- Procurement
- Government Contracting
- GovTech
- Market Intelligence
- Awards
- Opportunities
- Agents
---
