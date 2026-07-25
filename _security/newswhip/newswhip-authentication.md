---
api_key_in:
- query
api_specs:
- filename: newswhip-articles-api-openapi.yml
  format: yaml
  label: NewsWhip Articles API
  slug: newswhip-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-articles-api-openapi.yml
- filename: newswhip-articlesbyhrefs-api-openapi.yml
  format: yaml
  label: NewsWhip ArticlesByHrefs API
  slug: newswhip-articlesbyhrefs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-articlesbyhrefs-api-openapi.yml
- filename: newswhip-content-api-openapi.yml
  format: yaml
  label: NewsWhip Content API
  slug: newswhip-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-content-api-openapi.yml
- filename: newswhip-fbinfluencers-api-openapi.yml
  format: yaml
  label: NewsWhip FbInfluencers API
  slug: newswhip-fbinfluencers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-fbinfluencers-api-openapi.yml
- filename: newswhip-fbposts-api-openapi.yml
  format: yaml
  label: NewsWhip FbPosts API
  slug: newswhip-fbposts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-fbposts-api-openapi.yml
- filename: newswhip-influencers-api-openapi.yml
  format: yaml
  label: NewsWhip Influencers API
  slug: newswhip-influencers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-influencers-api-openapi.yml
- filename: newswhip-local-api-openapi.yml
  format: yaml
  label: NewsWhip Local API
  slug: newswhip-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-local-api-openapi.yml
- filename: newswhip-publisher-api-openapi.yml
  format: yaml
  label: NewsWhip Publisher API
  slug: newswhip-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-publisher-api-openapi.yml
- filename: newswhip-rankings-api-openapi.yml
  format: yaml
  label: NewsWhip Rankings API
  slug: newswhip-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-rankings-api-openapi.yml
- filename: newswhip-region-api-openapi.yml
  format: yaml
  label: NewsWhip Region API
  slug: newswhip-region-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-region-api-openapi.yml
- filename: newswhip-search-api-openapi.yml
  format: yaml
  label: NewsWhip Search API
  slug: newswhip-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-search-api-openapi.yml
- filename: newswhip-social-api-openapi.yml
  format: yaml
  label: NewsWhip Social API
  slug: newswhip-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-social-api-openapi.yml
- filename: newswhip-statistics-api-openapi.yml
  format: yaml
  label: NewsWhip Statistics API
  slug: newswhip-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-statistics-api-openapi.yml
- filename: newswhip-stats-api-openapi.yml
  format: yaml
  label: NewsWhip Stats API
  slug: newswhip-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-stats-api-openapi.yml
- filename: newswhip-twitterinfluencers-api-openapi.yml
  format: yaml
  label: NewsWhip TwitterInfluencers API
  slug: newswhip-twitterinfluencers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-twitterinfluencers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Newswhip Authentication
name_suffix: Authentication
oauth_flows: []
overview: NewsWhip secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NewsWhip
provider_slug: newswhip
scheme_count: 1
schemes:
- description: All requests are authenticated with a NewsWhip API key passed as the query parameter `key`. Keys are issued by NewsWhip on request (API access is provisioned per customer); there is no OAuth or self-service key generation.
  in: query
  name: sec0
  parameter: key
  sources:
  - openapi/newswhip-openapi.yml
  type: apiKey
slug: newswhip-authentication
source_filename: newswhip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/newswhip-openapi.yml\ndocs: https://developer.newswhip.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\nschemes:\n- name: sec0\n  type: apiKey\n  in: query\n  parameter: key\n  description: All requests are authenticated with a NewsWhip API key passed as the query parameter `key`.\n    Keys are issued by NewsWhip on request (API access is provisioned per customer); there is no OAuth\n    or self-service key generation.\n  sources:\n  - openapi/newswhip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/authentication/newswhip-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Media Intelligence
- Social Media Analytics
- News
- Content Analytics
- Engagement Data
- Predictive Analytics
- Media Monitoring
---
