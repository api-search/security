---
api_key_in:
- header
api_specs:
- filename: salesgraph-audit-api-openapi.yml
  format: yaml
  label: Salesgraph Audit API
  slug: salesgraph-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-audit-api-openapi.yml
- filename: salesgraph-commands-api-openapi.yml
  format: yaml
  label: Salesgraph Commands API
  slug: salesgraph-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-commands-api-openapi.yml
- filename: salesgraph-runs-api-openapi.yml
  format: yaml
  label: Salesgraph Runs API
  slug: salesgraph-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-runs-api-openapi.yml
- filename: salesgraph-oms-api-openapi.yml
  format: yaml
  label: Salesgraph OMS API
  slug: salesgraph-oms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-oms-api-openapi.yml
- filename: salesgraph-status-api-openapi.yml
  format: yaml
  label: Salesgraph Status API
  slug: salesgraph-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-status-api-openapi.yml
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
  - openapi/_original/salesgraph-openapi.yml
  type: http
- description: 'Alternative header — send your Salesgraph API key as `x-api-key: sg_live_...`.'
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/_original/salesgraph-openapi.yml
  type: apiKey
slug: salesgraph-authentication
source_filename: salesgraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.salesgraph.com/authentication\ndocs: https://docs.salesgraph.com/authentication\nkey_format: sg_live_ prefix; shown once at creation; created at dashboard Settings -> API Keys; non-expiring but revocable\nkey_management_url: https://salesgraph.com/dashboard/settings/api-keys\nkey_display_after_creation: short prefix only (e.g. sg_live_ab12...)\nrevocation: immediate\nguidance: use a separate key per integration or environment so one can be revoked in isolation\nunauthorized_response:\n  status: 401\n  body: '{ \"error\": \"unauthorized\" }'\n  header: 'WWW-Authenticate: Bearer'\n  observed: '2026-08-13 against https://www.salesgraph.com/api/mcp'\noauth: false\noauth_note: >\n  No OAuth or OIDC anywhere on the surface — /.well-known/oauth-authorization-server,\n  /oauth-protected-resource and /openid-configuration are all unserved, and the MCP server\n  answers a static bearer API key rather than an OAuth challenge.\
  \ No scopes/ artifact is written\n  because there is no scope surface to record. End-user login to the Salesgraph app itself uses\n  hosted WorkOS AuthKit, which is not part of the API contract.\npublic_operations:\n  - operation: getPlatformStatus\n    path: /api/status\n    spec: openapi/salesgraph-status-api-openapi.yml\n    note: The only documented operation that requires no credential.\nscope: per-organization; async run ids are org-isolated\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send your Salesgraph API key as `Authorization: Bearer sg_live_...`.'\n  sources:\n  - openapi/_original/salesgraph-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Alternative header — send your Salesgraph API key as `x-api-key: sg_live_...`.'\n  sources:\n  - openapi/_original/salesgraph-openapi.yml\n"
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
