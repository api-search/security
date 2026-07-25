---
api_key_in:
- header
api_specs:
- filename: bing-news-news-category-api-openapi.yml
  format: yaml
  label: Bing News Search News Category API
  slug: bing-news-news-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bing-news/refs/heads/main/openapi/bing-news-news-category-api-openapi.yml
- filename: bing-news-news-search-api-openapi.yml
  format: yaml
  label: Bing News Search News Search API
  slug: bing-news-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bing-news/refs/heads/main/openapi/bing-news-news-search-api-openapi.yml
- filename: bing-news-trending-topics-api-openapi.yml
  format: yaml
  label: Bing News Search Trending Topics API
  slug: bing-news-trending-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bing-news/refs/heads/main/openapi/bing-news-trending-topics-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bing News Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bing News Search secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bing News Search
provider_slug: bing-news
scheme_count: 1
schemes:
- description: The subscription key received when signing up for the Bing News Search service in the Azure Portal.
  in: header
  name: ApiKeyAuth
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/bing-news-search-openapi.json
  type: apiKey
slug: bing-news-authentication
source_filename: bing-news-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bing-news-search-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: The subscription key received when signing up for the Bing News Search service\n    in the Azure Portal.\n  sources:\n  - openapi/bing-news-search-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bing-news/refs/heads/main/authentication/bing-news-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Search
- Microsoft
- Bing
- Media
- Headlines
- Trending Topics
---
