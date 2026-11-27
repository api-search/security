---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: goodtiming-ai-metrics-api-openapi.yml
  format: yaml
  label: Good Timing Metrics API
  slug: goodtiming-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodtiming-ai/openapi/goodtiming-ai-metrics-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Good Timing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Good Timing secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Good Timing
provider_slug: goodtiming-ai
scheme_count: 3
schemes:
- description: '''Bearer <your API key>''.'
  in: header
  name: BearerApiKey
  parameter: Authorization
  sources:
  - openapi/goodtiming-ai-openapi.yml
  type: apiKey
- description: 'Auth key: the tenant identifier the Bearer token belongs to.'
  in: header
  name: TenantId
  parameter: x-baton-tenant-id
  sources:
  - openapi/goodtiming-ai-openapi.yml
  type: apiKey
- description: Per-server DSN carrying a publishable key (baton_pk_…), the events host, the workspace id (ten_…) and the server id (srv-…). HttpSink posts batches to {url}/v0/events/batch with the key as a bearer token. "A publishable key can only write events, and only for the server its DSN names, so it is safe in your source."
  in: header
  key_prefixes:
  - baton_pk_
  name: PublishableKeyDSN
  obtain: Sign in at baton.goodtiming.ai/account and press Add a server; DSNs are listed under Publishable keys.
  parameter: Authorization
  sources:
  - https://goodtiming.ai/docs.html
  type: apiKey
slug: goodtiming-ai-authentication
source_filename: goodtiming-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: searched\nsource:\n- https://goodtiming.ai/docs.html\n- openapi/goodtiming-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '''Bearer <your API key>''.'\n  sources:\n  - openapi/goodtiming-ai-openapi.yml\n- name: TenantId\n  type: apiKey\n  in: header\n  parameter: x-baton-tenant-id\n  description: 'Auth key: the tenant identifier the Bearer token belongs to.'\n  sources:\n  - openapi/goodtiming-ai-openapi.yml\n- name: PublishableKeyDSN\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Per-server DSN carrying a publishable key (baton_pk_…), the events host, the workspace id (ten_…) and the server id (srv-…). HttpSink posts batches to {url}/v0/events/batch with the key as\n    a bearer token. \"A publishable key can only write events, and only for the server its DSN names, so it is safe in\
  \ your source.\"\n  key_prefixes:\n  - baton_pk_\n  obtain: Sign in at baton.goodtiming.ai/account and press Add a server; DSNs are listed under Publishable keys.\n  sources:\n  - https://goodtiming.ai/docs.html\ndocs: https://goodtiming.ai/docs.html\nnotes:\n- Console API keys for the proxy sink are shown with prefix bk_live_ (BATON_API_KEY example \"bk_live_...\"); tenant id sent as BATON_TENANT_ID / x-baton-tenant-id.\n- No OAuth scopes are documented.\n"
source_yaml_url: https://artifacts.apis.io/goodtiming-ai/authentication/goodtiming-ai-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- MCP
- Product Analytics
- AI Agents
- Observability
- SDK
---
