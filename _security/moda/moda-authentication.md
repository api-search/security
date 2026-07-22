---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moda secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moda
provider_slug: moda
scheme_count: 2
schemes:
- format: Bearer <MODA_API_KEY>
  header: Authorization
  in: header
  name: IngestBearer
  scheme: bearer
  source: https://docs.moda.dev/ingestion/direct-api
  type: http
  used_by: Moda Ingestion API (POST /v1/ingest)
- env: MODA_API_KEY
  in: header
  name: x-api-key
  source: https://docs.moda.dev/data-api/overview
  type: apiKey
  used_by: Moda Data API + CLI + MCP server
slug: moda-authentication
source_filename: moda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.moda.dev/ingestion/direct-api\ndocs: https://docs.moda.dev/data-api/overview\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_prefix: moda_sk_\n  key_management: https://moda.dev/settings\n  oauth2_flows: []\nnotes: >-\n  Moda authenticates with a single tenant API key (prefix moda_sk_) obtained from\n  Settings at https://moda.dev/settings. The Ingestion API presents the key as an\n  HTTP Bearer credential; the read-only Data API and CLI present the same key via\n  the x-api-key header or the MODA_API_KEY environment variable. No OAuth2 / OpenID\n  Connect scope surface is documented, so there is no scopes/ artifact.\nschemes:\n- name: IngestBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Bearer <MODA_API_KEY>\"\n  used_by: Moda Ingestion API (POST /v1/ingest)\n  source: https://docs.moda.dev/ingestion/direct-api\n- name: DataApiKey\n  type: apiKey\n  in:\
  \ header\n  name: x-api-key\n  env: MODA_API_KEY\n  used_by: Moda Data API + CLI + MCP server\n  source: https://docs.moda.dev/data-api/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moda/refs/heads/main/authentication/moda-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- LLM Observability
- Agent Analytics
- Continual Learning
- Monitoring
- Developer Tools
- MCP
- OpenTelemetry
- Prompt Management
- Y Combinator
---
