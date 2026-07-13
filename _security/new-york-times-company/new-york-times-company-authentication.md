---
api_key_in:
- query
api_specs:
- filename: article-search-v2-openapi.yml
  format: yaml
  label: Article Search API
  slug: article-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/article-search-v2-openapi.yml
- filename: top-stories-v2-openapi.yml
  format: yaml
  label: Top Stories API
  slug: top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/top-stories-v2-openapi.yml
- filename: most-popular-api-v2-openapi.yml
  format: yaml
  label: Most Popular API
  slug: most-popular-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/most-popular-api-v2-openapi.yml
- filename: timeswire-v3-openapi.yml
  format: yaml
  label: Times Newswire API
  slug: times-newswire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/timeswire-v3-openapi.yml
- filename: archive-api-openapi.yml
  format: yaml
  label: Archive API
  slug: archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/archive-api-openapi.yml
- filename: books-api-openapi.yml
  format: yaml
  label: Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/books-api-openapi.yml
- filename: movie-reviews-v2-openapi.yml
  format: yaml
  label: Movie Reviews API
  slug: movie-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/movie-reviews-v2-openapi.yml
- filename: times-tags-v3-openapi.yml
  format: yaml
  label: TimesTags API
  slug: timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/times-tags-v3-openapi.yml
- filename: semantic-api-openapi.yml
  format: yaml
  label: Semantic API
  slug: semantic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/semantic-api-openapi.yml
- filename: geo-api-v2-openapi.yml
  format: yaml
  label: Geographic API
  slug: geographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/geo-api-v2-openapi.yml
- filename: community-api-v3-openapi.yml
  format: yaml
  label: Community API (Deprecated)
  slug: community-api-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-times-company/refs/heads/main/openapi/community-api-v3-openapi.yml
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
