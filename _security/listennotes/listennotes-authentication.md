---
api_key_in:
- header
api_specs:
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Search API
  slug: listennotes-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Typeahead API
  slug: listennotes-typeahead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Trending & Related Searches API
  slug: listennotes-trending-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Podcasts API
  slug: listennotes-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Episodes API
  slug: listennotes-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Best Podcasts API
  slug: listennotes-best-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Curated Lists API
  slug: listennotes-curated-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Playlists API
  slug: listennotes-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Genres, Regions & Languages API
  slug: listennotes-genres-regions-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Recommendations API
  slug: listennotes-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Podcast Audience Insights API
  slug: listennotes-audience-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
- filename: listennotes-openapi.yml
  format: yaml
  label: Listen Notes Podcaster API
  slug: listennotes-podcaster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Listennotes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listen Notes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Listen Notes
provider_slug: listennotes
scheme_count: 1
schemes:
- description: Your Listen API key, sent in the X-ListenAPI-Key request header.
  in: header
  name: apiKeyHeader
  parameter: X-ListenAPI-Key
  sources:
  - openapi/listennotes-openapi.yml
  type: apiKey
slug: listennotes-authentication
source_filename: listennotes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/listennotes-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-ListenAPI-Key\n  description: Your Listen API key, sent in the X-ListenAPI-Key request header.\n  sources:\n  - openapi/listennotes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/authentication/listennotes-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasts
- Podcast Search
- Podcast Directory
- Search
- Audio
- Media
- Podcast Insights
---
