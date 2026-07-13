---
api_key_in: []
api_specs:
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Filing Query API
  slug: sec-api-filing-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Full-Text Search API
  slug: sec-api-full-text-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-asyncapi.yml
  format: yaml
  label: SEC API Filing Stream API
  slug: sec-api-filing-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/asyncapi/sec-api-asyncapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API XBRL-to-JSON Converter API
  slug: sec-api-xbrl-to-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Extractor API
  slug: sec-api-extractor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Insider Trading API
  slug: sec-api-insider-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Form 13F Holdings API
  slug: sec-api-form-13f-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Sec Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: SEC API secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SEC API
provider_slug: sec-api
scheme_count: 3
schemes:
- description: 'REST calls authenticate with a single API token from your sec-api.io account, passed directly in the Authorization header with no `Bearer` prefix, e.g. `Authorization: YOUR_API_KEY`.'
  in: header
  name: apiKeyHeader
  scheme: Authorization
  sources:
  - https://sec-api.io/docs/query-api
  - openapi/sec-api-openapi.yml
  type: apiKey
- description: 'Alternative for REST calls: pass the same API token as the `token` query parameter, e.g. `https://api.sec-api.io?token=YOUR_API_KEY`.'
  in: query
  name: apiKeyQuery
  scheme: token
  sources:
  - https://sec-api.io/docs/query-api
  - openapi/sec-api-openapi.yml
  type: apiKey
- description: The real-time Filing Stream WebSocket authenticates with the token as the `apiKey` query parameter on the connection URL, e.g. `wss://stream.sec-api.io?apiKey=YOUR_API_KEY`.
  in: query
  name: apiKeyWebSocket
  scheme: apiKey
  sources:
  - https://sec-api.io/docs/stream-api
  - asyncapi/sec-api-asyncapi.yml
  type: apiKey
slug: sec-api-authentication
source_filename: sec-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: documented\nsource: https://sec-api.io/docs (query-api, full-text-search, stream-api)\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  scheme: Authorization\n  description: >-\n    REST calls authenticate with a single API token from your sec-api.io\n    account, passed directly in the Authorization header with no `Bearer`\n    prefix, e.g. `Authorization: YOUR_API_KEY`.\n  sources:\n  - https://sec-api.io/docs/query-api\n  - openapi/sec-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  scheme: token\n  description: >-\n    Alternative for REST calls: pass the same API token as the `token` query\n    parameter, e.g. `https://api.sec-api.io?token=YOUR_API_KEY`.\n  sources:\n  - https://sec-api.io/docs/query-api\n  - openapi/sec-api-openapi.yml\n- name: apiKeyWebSocket\n  type: apiKey\n  in: query\n  scheme: apiKey\n  description: >-\n    The real-time Filing Stream WebSocket authenticates\
  \ with the token as the\n    `apiKey` query parameter on the connection URL, e.g.\n    `wss://stream.sec-api.io?apiKey=YOUR_API_KEY`.\n  sources:\n  - https://sec-api.io/docs/stream-api\n  - asyncapi/sec-api-asyncapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/authentication/sec-api-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- SEC Filings
- Regulatory Filings
- EDGAR
- Financial Data
- Compliance
- Government Reports
- Insider Trading
- 13F
- XBRL
- Full-Text Search
---
