---
api_key_in: []
api_specs:
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Search News API
  slug: worldnewsapi-search-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Geo Coordinates API
  slug: worldnewsapi-geo-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Top News API
  slug: worldnewsapi-top-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Extract News API
  slug: worldnewsapi-extract-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Retrieve News API
  slug: worldnewsapi-retrieve-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Sources API
  slug: worldnewsapi-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Front Pages API
  slug: worldnewsapi-front-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Worldnewsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: World News API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: World News API
provider_slug: worldnewsapi
scheme_count: 2
schemes:
- description: API key passed as the "api-key" query parameter, e.g. https://api.worldnewsapi.com/search-news?text=news&api-key=YOUR_API_KEY. Obtain a key by signing up for a free account in the API console.
  in: query
  name: apiKeyQuery
  parameterName: api-key
  sources:
  - openapi/worldnewsapi-openapi.yml
  type: apiKey
- description: The same API key may instead be passed as the "x-api-key" HTTP request header.
  in: header
  name: apiKeyHeader
  parameterName: x-api-key
  sources:
  - openapi/worldnewsapi-openapi.yml
  type: apiKey
slug: worldnewsapi-authentication
source_filename: worldnewsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/worldnewsapi-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameterName: api-key\n  description: >-\n    API key passed as the \"api-key\" query parameter, e.g.\n    https://api.worldnewsapi.com/search-news?text=news&api-key=YOUR_API_KEY.\n    Obtain a key by signing up for a free account in the API console.\n  sources:\n  - openapi/worldnewsapi-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameterName: x-api-key\n  description: >-\n    The same API key may instead be passed as the \"x-api-key\" HTTP request\n    header.\n  sources:\n  - openapi/worldnewsapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/authentication/worldnewsapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- News
- Local News
- News Search
- Media Monitoring
- Geo Search
- News Data
- Sentiment Analysis
- Content Extraction
---
