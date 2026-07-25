---
api_key_in: []
api_specs:
- filename: aligned-news-bundles-api-openapi.yml
  format: yaml
  label: Aligned News Bundles API
  slug: aligned-news-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-bundles-api-openapi.yml
- filename: aligned-news-news-feed-api-openapi.yml
  format: yaml
  label: Aligned News News Feed API
  slug: aligned-news-news-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-news-feed-api-openapi.yml
- filename: aligned-news-reports-api-openapi.yml
  format: yaml
  label: Aligned News Reports API
  slug: aligned-news-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-reports-api-openapi.yml
- filename: aligned-news-search-api-openapi.yml
  format: yaml
  label: Aligned News Search API
  slug: aligned-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-search-api-openapi.yml
- filename: aligned-news-sections-api-openapi.yml
  format: yaml
  label: Aligned News Sections API
  slug: aligned-news-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-sections-api-openapi.yml
- filename: aligned-news-signals-api-openapi.yml
  format: yaml
  label: Aligned News Signals API
  slug: aligned-news-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-signals-api-openapi.yml
- filename: aligned-news-stories-api-openapi.yml
  format: yaml
  label: Aligned News Stories API
  slug: aligned-news-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/openapi/aligned-news-stories-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aligned News Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aligned News secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aligned News
provider_slug: aligned-news
scheme_count: 1
schemes:
- bearerFormat: alnw_*
  description: API key issued from https://alignednews.com/account, presented as Authorization Bearer [example key]
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aligned-news-openapi.yml
  type: http
slug: aligned-news-authentication
source_filename: aligned-news-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aligned-news-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: alnw_*\n  description: API key issued from https://alignednews.com/account, presented as Authorization\n    Bearer [example key]\n  sources:\n  - openapi/aligned-news-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aligned-news/refs/heads/main/authentication/aligned-news-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- News
- Intelligence
- MCP
- Signals
---
