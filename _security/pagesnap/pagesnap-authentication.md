---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: pagesnap-account-api-openapi.yml
  format: yaml
  label: Pagesnap Account API
  slug: pagesnap-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-account-api-openapi.yml
- filename: pagesnap-agents-api-openapi.yml
  format: yaml
  label: Pagesnap Agents API
  slug: pagesnap-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-agents-api-openapi.yml
- filename: pagesnap-billing-api-openapi.yml
  format: yaml
  label: Pagesnap Billing API
  slug: pagesnap-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-billing-api-openapi.yml
- filename: pagesnap-content-api-openapi.yml
  format: yaml
  label: Pagesnap Content API
  slug: pagesnap-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-content-api-openapi.yml
- filename: pagesnap-crawl-api-openapi.yml
  format: yaml
  label: Pagesnap Crawl API
  slug: pagesnap-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-crawl-api-openapi.yml
- filename: pagesnap-diff-api-openapi.yml
  format: yaml
  label: Pagesnap Diff API
  slug: pagesnap-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-diff-api-openapi.yml
- filename: pagesnap-discovery-api-openapi.yml
  format: yaml
  label: Pagesnap Discovery API
  slug: pagesnap-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-discovery-api-openapi.yml
- filename: pagesnap-monitors-api-openapi.yml
  format: yaml
  label: Pagesnap Monitors API
  slug: pagesnap-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-monitors-api-openapi.yml
- filename: pagesnap-status-api-openapi.yml
  format: yaml
  label: Pagesnap Status API
  slug: pagesnap-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-status-api-openapi.yml
- filename: pagesnap-support-api-openapi.yml
  format: yaml
  label: Pagesnap Support API
  slug: pagesnap-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-support-api-openapi.yml
- filename: pagesnap-x402-api-openapi.yml
  format: yaml
  label: Pagesnap X402 API
  slug: pagesnap-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-x402-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
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
- Developer Tools
- Web Scraping
- web-to-markdown
- screenshot-api
- PDF Generation
- Metadata Extraction
- MCP
- A2A
- x402
- AI Agents
- Content Extraction
- Structured Data
- Web Crawling
- Change Monitoring
- llms-txt
- Agentic Payments
- Software-as-a-Service
---
