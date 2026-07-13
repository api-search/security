---
api_key_in:
- header
- query
api_specs:
- filename: newsapi-newsapi-openapi.yml
  format: yaml
  label: NewsAPI
  slug: newsapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsapi/refs/heads/main/openapi/newsapi-newsapi-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Newsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: NewsAPI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NewsAPI
provider_slug: newsapi
scheme_count: 3
schemes:
- description: API key passed via X-Api-Key HTTP header
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/newsapi-newsapi-openapi.yml
  type: apiKey
- description: API key passed as a query parameter
  in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/newsapi-newsapi-openapi.yml
  type: apiKey
- description: 'API key passed as a Bearer token. Note: the Bearer prefix is optional and the key should NOT be base64 encoded.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/newsapi-newsapi-openapi.yml
  type: http
slug: newsapi-authentication
source_filename: newsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/newsapi-newsapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key passed via X-Api-Key HTTP header\n  sources:\n  - openapi/newsapi-newsapi-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key passed as a query parameter\n  sources:\n  - openapi/newsapi-newsapi-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key passed as a Bearer token. Note: the Bearer prefix is optional and the\n    key should NOT be base64 encoded.'\n  sources:\n  - openapi/newsapi-newsapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newsapi/refs/heads/main/authentication/newsapi-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- News
- Headlines
- Articles
- Search
- Media
- Content
- REST
- JSON
---
