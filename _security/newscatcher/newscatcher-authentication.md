---
api_key_in:
- header
api_specs:
- filename: newscatcher-news-api-openapi.yml
  format: yaml
  label: Newscatcher News API
  slug: news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-news-api-openapi.yml
- filename: newscatcher-web-search-api-openapi.yml
  format: yaml
  label: Newscatcher CatchAll Web Search API
  slug: web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-web-search-api-openapi.yml
- filename: newscatcher-local-news-api-openapi.yml
  format: yaml
  label: Newscatcher Local News API
  slug: local-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-local-news-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Newscatcher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Newscatcher secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Newscatcher
provider_slug: newscatcher
scheme_count: 2
schemes:
- description: "API Key to authenticate requests.\n\nTo access the API, include your API key in the `x-api-token` header. \nTo obtain your API key, complete the [form](https://www.newscatcherapi.com/book-a-demo) or contact us directly."
  in: header
  name: ApiKeyAuth
  parameter: x-api-token
  sources:
  - openapi/newscatcher-local-news-api-openapi.yml
  - openapi/newscatcher-news-api-openapi.yml
  type: apiKey
- description: API key for authentication.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/newscatcher-web-search-api-openapi.yml
  type: apiKey
slug: newscatcher-authentication
source_filename: newscatcher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/newscatcher-local-news-api-openapi.yml, openapi/newscatcher-news-api-openapi.yml,\n  openapi/newscatcher-web-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  description: \"API Key to authenticate requests.\\n\\nTo access the API, include your API key\\\n    \\ in the `x-api-token` header. \\nTo obtain your API key, complete the [form](https://www.newscatcherapi.com/book-a-demo)\\\n    \\ or contact us directly.\"\n  sources:\n  - openapi/newscatcher-local-news-api-openapi.yml\n  - openapi/newscatcher-news-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication.\n  sources:\n  - openapi/newscatcher-web-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/authentication/newscatcher-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- News
- Search
- NLP
- Sentiment Analysis
- Entity Extraction
- Clustering
- Media Intelligence
- Financial Intelligence
- AI
- Enterprise
---
