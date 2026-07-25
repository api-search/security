---
api_key_in:
- query
api_specs:
- filename: new-york-times-company-archive-api-openapi.yml
  format: yaml
  label: The New York Times Company Archive API
  slug: new-york-times-company-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-archive-api-openapi.yml
- filename: new-york-times-company-content-api-openapi.yml
  format: yaml
  label: The New York Times Company Content API
  slug: new-york-times-company-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-content-api-openapi.yml
- filename: new-york-times-company-content-json-api-openapi.yml
  format: yaml
  label: The New York Times Company Content.json API
  slug: new-york-times-company-content-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-content-json-api-openapi.yml
- filename: new-york-times-company-events-api-openapi.yml
  format: yaml
  label: The New York Times Company Events API
  slug: new-york-times-company-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-events-api-openapi.yml
- filename: new-york-times-company-lists-api-openapi.yml
  format: yaml
  label: The New York Times Company Lists API
  slug: new-york-times-company-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-lists-api-openapi.yml
- filename: new-york-times-company-lists-json-api-openapi.yml
  format: yaml
  label: The New York Times Company Lists.json API
  slug: new-york-times-company-lists-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-lists-json-api-openapi.yml
- filename: new-york-times-company-most-popular-api-openapi.yml
  format: yaml
  label: The New York Times Company Most Popular API
  slug: new-york-times-company-most-popular-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-most-popular-api-openapi.yml
- filename: new-york-times-company-movies-api-openapi.yml
  format: yaml
  label: The New York Times Company Movies API
  slug: new-york-times-company-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-movies-api-openapi.yml
- filename: new-york-times-company-name-api-openapi.yml
  format: yaml
  label: The New York Times Company Name API
  slug: new-york-times-company-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-name-api-openapi.yml
- filename: new-york-times-company-reviews-json-api-openapi.yml
  format: yaml
  label: The New York Times Company Reviews.json API
  slug: new-york-times-company-reviews-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-reviews-json-api-openapi.yml
- filename: new-york-times-company-search-api-openapi.yml
  format: yaml
  label: The New York Times Company Search API
  slug: new-york-times-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-search-api-openapi.yml
- filename: new-york-times-company-search-json-api-openapi.yml
  format: yaml
  label: The New York Times Company Search.json API
  slug: new-york-times-company-search-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-search-json-api-openapi.yml
- filename: new-york-times-company-stories-api-openapi.yml
  format: yaml
  label: The New York Times Company Stories API
  slug: new-york-times-company-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-stories-api-openapi.yml
- filename: new-york-times-company-timestags-api-openapi.yml
  format: yaml
  label: The New York Times Company Timestags API
  slug: new-york-times-company-timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-timestags-api-openapi.yml
- filename: new-york-times-company-user-content-api-openapi.yml
  format: yaml
  label: The New York Times Company User Content API
  slug: new-york-times-company-user-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/new-york-times-company-user-content-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: New York Times Company Authentication
name_suffix: Authentication
oauth_flows: []
overview: The New York Times Company secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The New York Times Company
provider_slug: new-york-times-company
scheme_count: 1
schemes:
- in: query
  name: apikey
  parameter: api-key
  sources:
  - openapi/archive-api-openapi.yml
  - openapi/article-search-v2-openapi.yml
  - openapi/books-api-openapi.yml
  - openapi/community-api-v3-openapi.yml
  - openapi/geo-api-v2-openapi.yml
  - openapi/most-popular-api-v2-openapi.yml
  - openapi/movie-reviews-v2-openapi.yml
  - openapi/semantic-api-openapi.yml
  - openapi/times-tags-v3-openapi.yml
  - openapi/timeswire-v3-openapi.yml
  - openapi/top-stories-v2-openapi.yml
  type: apiKey
slug: new-york-times-company-authentication
source_filename: new-york-times-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/archive-api-openapi.yml, openapi/article-search-v2-openapi.yml, openapi/books-api-openapi.yml,\n  openapi/community-api-v3-openapi.yml, openapi/geo-api-v2-openapi.yml, openapi/most-popular-api-v2-openapi.yml,\n  openapi/movie-reviews-v2-openapi.yml, openapi/semantic-api-openapi.yml, openapi/times-tags-v3-openapi.yml,\n  openapi/timeswire-v3-openapi.yml, openapi/top-stories-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/archive-api-openapi.yml\n  - openapi/article-search-v2-openapi.yml\n  - openapi/books-api-openapi.yml\n  - openapi/community-api-v3-openapi.yml\n  - openapi/geo-api-v2-openapi.yml\n  - openapi/most-popular-api-v2-openapi.yml\n  - openapi/movie-reviews-v2-openapi.yml\n  - openapi/semantic-api-openapi.yml\n  - openapi/times-tags-v3-openapi.yml\n  - openapi/timeswire-v3-openapi.yml\n\
  \  - openapi/top-stories-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/authentication/new-york-times-company-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Media
- Publishing
- Newspapers
- Articles
- Books
- Movies
- Sports
- Games
- Cooking
- Reviews
- Search
- Semantic
- Tagging
- Controlled Vocabulary
- Geographic
- Archive
---
