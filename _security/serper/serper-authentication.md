---
api_key_in:
- header
api_specs:
- filename: serper-autocomplete-api-openapi.yml
  format: yaml
  label: Serper Autocomplete API
  slug: serper-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-autocomplete-api-openapi.yml
- filename: serper-images-api-openapi.yml
  format: yaml
  label: Serper Images API
  slug: serper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-images-api-openapi.yml
- filename: serper-maps-api-openapi.yml
  format: yaml
  label: Serper Maps API
  slug: serper-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-maps-api-openapi.yml
- filename: serper-news-api-openapi.yml
  format: yaml
  label: Serper News API
  slug: serper-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-news-api-openapi.yml
- filename: serper-patents-api-openapi.yml
  format: yaml
  label: Serper Patents API
  slug: serper-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-patents-api-openapi.yml
- filename: serper-places-api-openapi.yml
  format: yaml
  label: Serper Places API
  slug: serper-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-places-api-openapi.yml
- filename: serper-scholar-api-openapi.yml
  format: yaml
  label: Serper Scholar API
  slug: serper-scholar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-scholar-api-openapi.yml
- filename: serper-search-api-openapi.yml
  format: yaml
  label: Serper Search API
  slug: serper-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-search-api-openapi.yml
- filename: serper-shopping-api-openapi.yml
  format: yaml
  label: Serper Shopping API
  slug: serper-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-shopping-api-openapi.yml
- filename: serper-videos-api-openapi.yml
  format: yaml
  label: Serper Videos API
  slug: serper-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-videos-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Serper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Serper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Serper
provider_slug: serper
scheme_count: 1
schemes:
- description: API key obtained from https://serper.dev/api-key
  in: header
  name: apiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/serper-google-search-api-openapi.yml
  type: apiKey
slug: serper-authentication
source_filename: serper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/serper-google-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key obtained from https://serper.dev/api-key\n  sources:\n  - openapi/serper-google-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/authentication/serper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- SERP
- Google Search
- AI
- LLM
- SEO
- Images
- News
- Maps
- Shopping
---
