---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Finlight Financial News API
  slug: finlight-financial-news-api
  spec_type: OpenAPI
  url: https://docs.finlight.me/v2/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Finlight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finlight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finlight
provider_slug: finlight
scheme_count: 1
schemes:
- description: API key obtained from https://app.finlight.me
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/openapi.json
  type: apiKey
slug: finlight-authentication
source_filename: finlight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key obtained from https://app.finlight.me\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finlight/refs/heads/main/authentication/finlight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial News
- Sentiment Analysis
- Market Data
- Equities
- Currencies
- Commodities
- Real-Time
- Webhooks
- WebSocket
---
