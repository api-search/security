---
api_key_in:
- query
- header
api_specs:
- filename: searchapi-search-api-openapi.yml
  format: yaml
  label: SearchApi SERP API
  slug: searchapi-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-search-api-openapi.yml
- filename: searchapi-account-api-openapi.yml
  format: yaml
  label: SearchApi Account & Analytics API
  slug: searchapi-account-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-account-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Searchapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SearchApi secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SearchApi
provider_slug: searchapi
scheme_count: 3
schemes:
- description: API key supplied as the `api_key` query-string parameter.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - https://www.searchapi.io/docs/google
  type: apiKey
- bearerFormat: opaque
  description: 'API key supplied as an `Authorization: Bearer <API_KEY>` header.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://www.searchapi.io/docs/google
  type: http
- description: Hosted MCP server token (the same account API key); also accepted as a `?token=` query parameter. Obtain from the dashboard MCP integrations page.
  in: header
  name: McpToken
  parameter: X-MCP-Token
  sources:
  - https://www.searchapi.io/mcp
  type: apiKey
slug: searchapi-authentication
source_filename: searchapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.searchapi.io/docs/google\ndocs: https://www.searchapi.io/docs/google\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  note: >-\n    SearchApi uses a single API key. It may be supplied either as an `api_key`\n    query parameter or as an HTTP `Authorization: Bearer <API_KEY>` header. There\n    is no OAuth surface for the REST API. The hosted MCP server authenticates the\n    same key via a `?token=` query parameter or an `X-MCP-Token` request header.\nschemes:\n  - name: ApiKeyQuery\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: API key supplied as the `api_key` query-string parameter.\n    sources: [https://www.searchapi.io/docs/google]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: opaque\n    description: \"API key supplied as an `Authorization: Bearer <API_KEY>` header.\"\n    sources: [https://www.searchapi.io/docs/google]\n\
  \  - name: McpToken\n    type: apiKey\n    in: header\n    parameter: X-MCP-Token\n    description: >-\n      Hosted MCP server token (the same account API key); also accepted as a\n      `?token=` query parameter. Obtain from the dashboard MCP integrations page.\n    sources: [https://www.searchapi.io/mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/authentication/searchapi-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- search
- serp-api
- google-search
- web-scraping
- search-data
- market-intelligence
- seo
- mcp
- agent-native
---
