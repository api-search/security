---
api_key_in:
- header
- query
api_specs:
- filename: openapi.json
  format: json
  label: Pagesnap API
  slug: pagesnap-api
  spec_type: OpenAPI
  url: https://pagesnap.142-93-197-141.sslip.io/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pagesnap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pagesnap secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pagesnap
provider_slug: pagesnap
scheme_count: 4
schemes:
- bearerFormat: ps_live_…
  description: Pagesnap API key.
  name: bearer
  scheme: bearer
  sources:
  - openapi/pagesnap-openapi.json
  type: http
- in: header
  name: apiHeader
  parameter: X-API-Key
  sources:
  - openapi/pagesnap-openapi.json
  type: apiKey
- description: Compatibility only; headers avoid key leakage in URLs.
  in: query
  name: apiQuery
  parameter: key
  sources:
  - openapi/pagesnap-openapi.json
  type: apiKey
- description: x402 v2 exact EIP-3009 USDC authorization on Base; X-PAYMENT is a legacy alias.
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/pagesnap-openapi.json
  type: apiKey
slug: pagesnap-authentication
source_filename: pagesnap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/pagesnap-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: ps_live_…\n  description: Pagesnap API key.\n  sources:\n  - openapi/pagesnap-openapi.json\n- name: apiHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/pagesnap-openapi.json\n- name: apiQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Compatibility only; headers avoid key leakage in URLs.\n  sources:\n  - openapi/pagesnap-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 v2 exact EIP-3009 USDC authorization on Base; X-PAYMENT is a legacy alias.\n  sources:\n  - openapi/pagesnap-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/authentication/pagesnap-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- developer-tools
- web-scraping
- web-to-markdown
- screenshot-api
- pdf-generation
- metadata-extraction
- mcp
- a2a
- x402
- ai-agents
- content-extraction
- structured-data
- web-crawling
- change-monitoring
- llms-txt
- agent-payments
- saas
---
