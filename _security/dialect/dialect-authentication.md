---
api_key_in:
- header
api_specs:
- filename: dialect-blink-api-openapi.yml
  format: yaml
  label: Dialect Blink API
  slug: dialect-blink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-api-openapi.yml
- filename: dialect-blink-data-table-api-openapi.yml
  format: yaml
  label: Dialect Blink Data Table API
  slug: dialect-blink-data-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-data-table-api-openapi.yml
- filename: dialect-blink-lists-api-openapi.yml
  format: yaml
  label: Dialect Blink Lists API
  slug: dialect-blink-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-lists-api-openapi.yml
- filename: dialect-blink-preview-api-openapi.yml
  format: yaml
  label: Dialect Blink Preview API
  slug: dialect-blink-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-preview-api-openapi.yml
- filename: dialect-channels-api-openapi.yml
  format: yaml
  label: Dialect Channels API
  slug: dialect-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-channels-api-openapi.yml
- filename: dialect-inbox-api-openapi.yml
  format: yaml
  label: Dialect Inbox API
  slug: dialect-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-inbox-api-openapi.yml
- filename: dialect-markets-api-openapi.yml
  format: yaml
  label: Dialect Markets API
  slug: dialect-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-markets-api-openapi.yml
- filename: dialect-positions-api-openapi.yml
  format: yaml
  label: Dialect Positions API
  slug: dialect-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-positions-api-openapi.yml
- filename: dialect-send-api-openapi.yml
  format: yaml
  label: Dialect Send API
  slug: dialect-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-send-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dialect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dialect secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dialect
provider_slug: dialect
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: Bearer token authentication for subscriber calls.
  name: subscriber
  scheme: bearer
  sources:
  - openapi/dialect-alerts-openapi.json
  type: http
- description: API key to authorize app-level requests.
  in: header
  name: application
  parameter: x-dialect-api-key
  sources:
  - openapi/dialect-alerts-openapi.json
  type: apiKey
- description: Client key to authorize requests.
  in: header
  name: clientKey
  parameter: x-blink-client-key
  sources:
  - openapi/dialect-blinks-openapi.json
  type: apiKey
- description: Client key for the Markets API
  in: header
  name: apiKey
  parameter: x-dialect-client-key
  sources:
  - openapi/dialect-markets-openapi.json
  type: apiKey
slug: dialect-authentication
source_filename: dialect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/dialect-alerts-openapi.json, openapi/dialect-blinks-openapi.json, openapi/dialect-markets-openapi.json\ndocs:\n- https://docs.dialect.to/alerts/send/api/authentication\n- https://docs.dialect.to/alerts/integrate-inbox/api/authentication\n- https://docs.dialect.to/alerts/api-keys\nnotes: >-\n  Three key surfaces: app-level Alerts calls use x-dialect-api-key; Blinks calls use\n  x-blink-client-key; Markets calls use x-dialect-client-key (public demo key pk_demo).\n  Subscriber-scoped inbox calls use a JWT bearer obtained via Solana wallet\n  message/transaction signing (prepare -> sign -> verify).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: subscriber\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication for subscriber calls.\n  sources:\n  - openapi/dialect-alerts-openapi.json\n- name: application\n  type: apiKey\n  in: header\n  parameter:\
  \ x-dialect-api-key\n  description: API key to authorize app-level requests.\n  sources:\n  - openapi/dialect-alerts-openapi.json\n- name: clientKey\n  type: apiKey\n  in: header\n  parameter: x-blink-client-key\n  description: Client key to authorize requests.\n  sources:\n  - openapi/dialect-blinks-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-dialect-client-key\n  description: Client key for the Markets API\n  sources:\n  - openapi/dialect-markets-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/authentication/dialect-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Infrastructure
- Web3
- Blockchain
- Solana
- Notifications
- Messaging
- Alerts
- DeFi
- Payments
- Agents
- MCP
---
