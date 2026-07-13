---
api_key_in:
- header
api_specs:
- filename: alphasense-agent-api-openapi.yml
  format: yaml
  label: AlphaSense Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-agent-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Ingestion API
  slug: ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Companies API
  slug: companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Brokers API
  slug: brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Watchlist API
  slug: watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-agent-api-openapi.yml
  format: yaml
  label: AlphaSense Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-agent-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alphasense Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlphaSense secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AlphaSense
provider_slug: alphasense
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alphasense-agent-api-openapi.yml
  - openapi/alphasense-utility-api-openapi.yml
  type: http
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/alphasense-agent-api-openapi.yml
  - openapi/alphasense-utility-api-openapi.yml
  type: apiKey
slug: alphasense-authentication
source_filename: alphasense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alphasense-agent-api-openapi.yml, openapi/alphasense-utility-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/alphasense-agent-api-openapi.yml\n  - openapi/alphasense-utility-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/alphasense-agent-api-openapi.yml\n  - openapi/alphasense-utility-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/authentication/alphasense-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Market Intelligence
- Financial Research
- Search
- Generative AI
- AI Agents
- Expert Calls
- Document Intelligence
- Enterprise Intelligence
- MCP
- GraphQL
---
