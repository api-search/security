---
api_key_in:
- header
api_specs:
- filename: govly-tools-v1-openapi-original.yml
  format: yaml
  label: Govly Tools API
  slug: govly-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govly/refs/heads/main/openapi/govly-tools-v1-openapi-original.yml
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
