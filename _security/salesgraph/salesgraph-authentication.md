---
api_key_in:
- header
api_specs:
- filename: salesgraph-openapi.yml
  format: yaml
  label: Salesgraph REST API
  slug: salesgraph-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Salesgraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salesgraph secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Salesgraph
provider_slug: salesgraph
scheme_count: 2
schemes:
- description: 'Send your Salesgraph API key as `Authorization: Bearer sg_live_...`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesgraph-openapi.yml
  type: http
- description: 'Alternative header — send your Salesgraph API key as `x-api-key: sg_live_...`.'
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/salesgraph-openapi.yml
  type: apiKey
slug: salesgraph-authentication
source_filename: salesgraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/salesgraph-openapi.yml\ndocs: https://docs.salesgraph.com/authentication\nkey_format: sg_live_ prefix; shown once at creation; created at dashboard Settings -> API Keys; non-expiring but revocable\nscope: per-organization; async run ids are org-isolated\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send your Salesgraph API key as `Authorization: Bearer sg_live_...`.'\n  sources:\n  - openapi/salesgraph-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Alternative header — send your Salesgraph API key as `x-api-key: sg_live_...`.'\n  sources:\n  - openapi/salesgraph-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/authentication/salesgraph-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Sales
- Revenue Automation
- Go-To-Market
- AI Agents
- MCP
- Sales Intelligence
- Competitive Intelligence
- Research
- Enterprise Sales
---
