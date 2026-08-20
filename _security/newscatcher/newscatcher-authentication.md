---
api_key_in:
- header
api_specs:
- filename: newscatcher-aggregationcount-api-openapi.yml
  format: yaml
  label: Newscatcher AggregationCount API
  slug: newscatcher-aggregationcount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-aggregationcount-api-openapi.yml
- filename: newscatcher-authors-api-openapi.yml
  format: yaml
  label: Newscatcher Authors API
  slug: newscatcher-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-authors-api-openapi.yml
- filename: newscatcher-breakingnews-api-openapi.yml
  format: yaml
  label: Newscatcher BreakingNews API
  slug: newscatcher-breakingnews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-breakingnews-api-openapi.yml
- filename: newscatcher-datasets-api-openapi.yml
  format: yaml
  label: Newscatcher Datasets API
  slug: newscatcher-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-datasets-api-openapi.yml
- filename: newscatcher-entities-api-openapi.yml
  format: yaml
  label: Newscatcher Entities API
  slug: newscatcher-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-entities-api-openapi.yml
- filename: newscatcher-jobs-api-openapi.yml
  format: yaml
  label: Newscatcher Jobs API
  slug: newscatcher-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-jobs-api-openapi.yml
- filename: newscatcher-latestheadlines-api-openapi.yml
  format: yaml
  label: Newscatcher LatestHeadlines API
  slug: newscatcher-latestheadlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-latestheadlines-api-openapi.yml
- filename: newscatcher-meta-api-openapi.yml
  format: yaml
  label: Newscatcher Meta API
  slug: newscatcher-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-meta-api-openapi.yml
- filename: newscatcher-monitors-api-openapi.yml
  format: yaml
  label: Newscatcher Monitors API
  slug: newscatcher-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-monitors-api-openapi.yml
- filename: newscatcher-projects-api-openapi.yml
  format: yaml
  label: Newscatcher Projects API
  slug: newscatcher-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-projects-api-openapi.yml
- filename: newscatcher-search-api-openapi.yml
  format: yaml
  label: Newscatcher Search API
  slug: newscatcher-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-search-api-openapi.yml
- filename: newscatcher-searchby-api-openapi.yml
  format: yaml
  label: Newscatcher SearchBy API
  slug: newscatcher-searchby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-searchby-api-openapi.yml
- filename: newscatcher-searchbylink-api-openapi.yml
  format: yaml
  label: Newscatcher SearchByLink API
  slug: newscatcher-searchbylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-searchbylink-api-openapi.yml
- filename: newscatcher-sources-api-openapi.yml
  format: yaml
  label: Newscatcher Sources API
  slug: newscatcher-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-sources-api-openapi.yml
- filename: newscatcher-subscription-api-openapi.yml
  format: yaml
  label: Newscatcher Subscription API
  slug: newscatcher-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-subscription-api-openapi.yml
- filename: newscatcher-webhooks-api-openapi.yml
  format: yaml
  label: Newscatcher Webhooks API
  slug: newscatcher-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-webhooks-api-openapi.yml
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
- Artificial Intelligence
- Enterprise
---
