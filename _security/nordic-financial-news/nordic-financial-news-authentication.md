---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nordic-financial-news-articles-api-openapi.yml
  format: yaml
  label: Nordic Financial News Articles API
  slug: nordic-financial-news-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-articles-api-openapi.yml
- filename: nordic-financial-news-calendar-events-api-openapi.yml
  format: yaml
  label: Nordic Financial News Calendar Events API
  slug: nordic-financial-news-calendar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-calendar-events-api-openapi.yml
- filename: nordic-financial-news-categories-api-openapi.yml
  format: yaml
  label: Nordic Financial News Categories API
  slug: nordic-financial-news-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-categories-api-openapi.yml
- filename: nordic-financial-news-companies-api-openapi.yml
  format: yaml
  label: Nordic Financial News Companies API
  slug: nordic-financial-news-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-companies-api-openapi.yml
- filename: nordic-financial-news-countries-api-openapi.yml
  format: yaml
  label: Nordic Financial News Countries API
  slug: nordic-financial-news-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-countries-api-openapi.yml
- filename: nordic-financial-news-event-types-api-openapi.yml
  format: yaml
  label: Nordic Financial News Event Types API
  slug: nordic-financial-news-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-event-types-api-openapi.yml
- filename: nordic-financial-news-events-api-openapi.yml
  format: yaml
  label: Nordic Financial News Events API
  slug: nordic-financial-news-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-events-api-openapi.yml
- filename: nordic-financial-news-exchanges-api-openapi.yml
  format: yaml
  label: Nordic Financial News Exchanges API
  slug: nordic-financial-news-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-exchanges-api-openapi.yml
- filename: nordic-financial-news-health-api-openapi.yml
  format: yaml
  label: Nordic Financial News Health API
  slug: nordic-financial-news-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-health-api-openapi.yml
- filename: nordic-financial-news-indices-api-openapi.yml
  format: yaml
  label: Nordic Financial News Indices API
  slug: nordic-financial-news-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-indices-api-openapi.yml
- filename: nordic-financial-news-meta-api-openapi.yml
  format: yaml
  label: Nordic Financial News Meta API
  slug: nordic-financial-news-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-meta-api-openapi.yml
- filename: nordic-financial-news-search-api-openapi.yml
  format: yaml
  label: Nordic Financial News Search API
  slug: nordic-financial-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-search-api-openapi.yml
- filename: nordic-financial-news-sources-api-openapi.yml
  format: yaml
  label: Nordic Financial News Sources API
  slug: nordic-financial-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-sources-api-openapi.yml
- filename: nordic-financial-news-stories-api-openapi.yml
  format: yaml
  label: Nordic Financial News Stories API
  slug: nordic-financial-news-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-stories-api-openapi.yml
- filename: nordic-financial-news-watchlists-api-openapi.yml
  format: yaml
  label: Nordic Financial News Watchlists API
  slug: nordic-financial-news-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-watchlists-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nordic Financial News Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nordic Financial News secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nordic Financial News
provider_slug: nordic-financial-news
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: API Key authentication using Bearer token
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/nordic-financial-news-openapi.yml
  type: http
slug: nordic-financial-news-authentication
source_filename: nordic-financial-news-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/nordic-financial-news-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: API Key authentication using Bearer token\n  sources:\n  - openapi/nordic-financial-news-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/authentication/nordic-financial-news-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financial News
- Nordic
- Market Data
- Financial Calendar
- MCP
- News API
---
