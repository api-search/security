---
api_key_in:
- query
api_specs:
- filename: new-york-times-archive-openapi-original.yml
  format: yaml
  label: The New York Times Archive API
  slug: archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-archive-openapi-original.yml
- filename: new-york-times-article-search-openapi-original.yml
  format: yaml
  label: The New York Times Article Search API
  slug: article-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-article-search-openapi-original.yml
- filename: new-york-times-books-openapi-original.yml
  format: yaml
  label: The New York Times Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-books-openapi-original.yml
- filename: new-york-times-most-popular-openapi-original.yml
  format: yaml
  label: The New York Times Most Popular API
  slug: most-popular
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-most-popular-openapi-original.yml
- filename: new-york-times-movie-review-openapi-original.yml
  format: yaml
  label: The New York Times Movie Reviews API
  slug: movie-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-movie-review-openapi-original.yml
- filename: new-york-times-semantic-openapi-original.yml
  format: yaml
  label: The New York Times Semantic API
  slug: semantic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-semantic-openapi-original.yml
- filename: new-york-times-times-tags-openapi-original.yml
  format: yaml
  label: The New York Times TimesTags API
  slug: timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-times-tags-openapi-original.yml
- filename: new-york-times-times-newswire-openapi-original.yml
  format: yaml
  label: The New York Times Times Newswire API
  slug: times-newswire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-times-newswire-openapi-original.yml
- filename: new-york-times-top-stories-openapi-original.yml
  format: yaml
  label: The New York Times Top Stories API
  slug: top-stories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/new-york-times-top-stories-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The New York Times Authentication
name_suffix: Authentication
oauth_flows: []
overview: The New York Times secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The New York Times
provider_slug: the-new-york-times
scheme_count: 1
schemes:
- in: query
  name: apikey
  parameter: api-key
  sources:
  - openapi/new-york-times-archive-openapi-original.yml
  - openapi/new-york-times-article-search-openapi-original.yml
  - openapi/new-york-times-movie-review-openapi-original.yml
  - openapi/new-york-times-semantic-openapi-original.yml
  - openapi/new-york-times-times-newswire-openapi-original.yml
  - openapi/new-york-times-times-tags-openapi-original.yml
  - openapi/new-york-times-top-stories-openapi-original.yml
  type: apiKey
slug: the-new-york-times-authentication
source_filename: the-new-york-times-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/new-york-times-archive-openapi-original.yml, openapi/new-york-times-article-search-openapi-original.yml,\n  openapi/new-york-times-movie-review-openapi-original.yml, openapi/new-york-times-semantic-openapi-original.yml,\n  openapi/new-york-times-times-newswire-openapi-original.yml, openapi/new-york-times-times-tags-openapi-original.yml,\n  openapi/new-york-times-top-stories-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/new-york-times-archive-openapi-original.yml\n  - openapi/new-york-times-article-search-openapi-original.yml\n  - openapi/new-york-times-movie-review-openapi-original.yml\n  - openapi/new-york-times-semantic-openapi-original.yml\n  - openapi/new-york-times-times-newswire-openapi-original.yml\n  - openapi/new-york-times-times-tags-openapi-original.yml\n  - openapi/new-york-times-top-stories-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/authentication/the-new-york-times-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Articles
- Books
- Movies
- News
- Media
- Publishing
- Journalism
---
