---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentic-news-ai-agents-api-openapi.yml
  format: yaml
  label: Agentic News Agents API
  slug: agentic-news-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-agents-api-openapi.yml
- filename: agentic-news-ai-api-keys-api-openapi.yml
  format: yaml
  label: Agentic News API Keys API
  slug: agentic-news-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-api-keys-api-openapi.yml
- filename: agentic-news-ai-briefing-api-openapi.yml
  format: yaml
  label: Agentic News Briefing API
  slug: agentic-news-ai-briefing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-briefing-api-openapi.yml
- filename: agentic-news-ai-feed-api-openapi.yml
  format: yaml
  label: Agentic News Feed API
  slug: agentic-news-ai-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-feed-api-openapi.yml
- filename: agentic-news-ai-search-api-openapi.yml
  format: yaml
  label: Agentic News Search API
  slug: agentic-news-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-search-api-openapi.yml
- filename: agentic-news-ai-stories-api-openapi.yml
  format: yaml
  label: Agentic News Stories API
  slug: agentic-news-ai-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-stories-api-openapi.yml
- filename: agentic-news-ai-trending-api-openapi.yml
  format: yaml
  label: Agentic News Trending API
  slug: agentic-news-ai-trending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-trending-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentic News Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentic News secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agentic News
provider_slug: agentic-news-ai
scheme_count: 1
schemes:
- bearerFormat: API Key or OAuth Access Token
  description: 'API key starting with "ak_" or OAuth access token starting with "oa_". Create API keys at agentic-news.ai/settings/api-keys or via POST /api-keys with JWT auth. Pass as: Authorization: Bearer ak_...'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/agentic-news-ai-openapi.json
  type: http
slug: agentic-news-ai-authentication
source_filename: agentic-news-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentic-news-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API Key or OAuth Access Token\n  description: 'API key starting with \"ak_\" or OAuth access token starting with \"oa_\". Create\n    API keys at agentic-news.ai/settings/api-keys or via POST /api-keys with JWT auth. Pass\n    as: Authorization: Bearer ak_...'\n  sources:\n  - openapi/agentic-news-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentic-news-ai/authentication/agentic-news-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- News
- Aggregation
- DailyBriefings
- AI Agents
---
