---
api_key_in:
- query
api_specs:
- filename: the-new-york-times-archive-api-openapi.yml
  format: yaml
  label: The New York Times Archive API
  slug: the-new-york-times-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-archive-api-openapi.yml
- filename: the-new-york-times-content-api-openapi.yml
  format: yaml
  label: The New York Times Content API
  slug: the-new-york-times-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-content-api-openapi.yml
- filename: the-new-york-times-movies-api-openapi.yml
  format: yaml
  label: The New York Times Movies API
  slug: the-new-york-times-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-movies-api-openapi.yml
- filename: the-new-york-times-name-api-openapi.yml
  format: yaml
  label: The New York Times Name API
  slug: the-new-york-times-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-name-api-openapi.yml
- filename: the-new-york-times-search-api-openapi.yml
  format: yaml
  label: The New York Times Search API
  slug: the-new-york-times-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-search-api-openapi.yml
- filename: the-new-york-times-stories-api-openapi.yml
  format: yaml
  label: The New York Times Stories API
  slug: the-new-york-times-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-stories-api-openapi.yml
- filename: the-new-york-times-timestags-api-openapi.yml
  format: yaml
  label: The New York Times Timestags API
  slug: the-new-york-times-timestags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-new-york-times/refs/heads/main/openapi/the-new-york-times-timestags-api-openapi.yml
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
