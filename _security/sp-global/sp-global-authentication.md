---
api_key_in:
- cookie
api_specs:
- filename: kensho-llmready-openapi.yml
  format: yaml
  label: S&P Global LLM-Ready API (kFinance)
  slug: kensho-llm-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-llmready-openapi.yml
- filename: kensho-extract-openapi.yml
  format: yaml
  label: Kensho Extract API
  slug: kensho-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-extract-openapi.yml
- filename: kensho-nerd-openapi.yml
  format: yaml
  label: Kensho NERD API
  slug: kensho-nerd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-nerd-openapi.yml
- filename: kensho-scribe-batch-v2-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v2
  slug: kensho-scribe-batch-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-scribe-batch-v2-openapi.yml
- filename: kensho-scribe-realtime-asyncapi.yml
  format: yaml
  label: Kensho Scribe Real Time API
  slug: kensho-scribe-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/asyncapi/kensho-scribe-realtime-asyncapi.yml
- filename: kensho-scribe-batch-v1-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v1
  slug: kensho-scribe-batch-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-scribe-batch-v1-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sp Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: S&P Global secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: S&P Global
provider_slug: sp-global
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kensho-extract-openapi.yml
  - openapi/kensho-llmready-openapi.yml
  - openapi/kensho-nerd-openapi.yml
  - openapi/kensho-scribe-batch-v2-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/kensho-llmready-openapi.yml
  type: apiKey
- in: cookie
  name: APIKey
  parameter: kensho_nerd_token
  sources:
  - openapi/kensho-nerd-openapi.yml
  type: apiKey
slug: sp-global-authentication
source_filename: sp-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kensho-extract-openapi.yml, openapi/kensho-llmready-openapi.yml, openapi/kensho-nerd-openapi.yml,\n  openapi/kensho-scribe-batch-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/kensho-extract-openapi.yml\n  - openapi/kensho-llmready-openapi.yml\n  - openapi/kensho-nerd-openapi.yml\n  - openapi/kensho-scribe-batch-v2-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/kensho-llmready-openapi.yml\n- name: APIKey\n  type: apiKey\n  in: cookie\n  parameter: kensho_nerd_token\n  sources:\n  - openapi/kensho-nerd-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/authentication/sp-global-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Capital IQ
- Commodity Insights
- Credit Ratings
- Document Extraction
- ESG
- Financial Data
- Index Data
- LLM
- MCP
- Market Intelligence
- Mobility
- Named Entity Recognition
- Speech to Text
---
