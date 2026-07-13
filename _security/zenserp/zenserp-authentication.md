---
api_key_in:
- header
- query
api_specs:
- filename: documentation
  format: yaml
  label: Zenserp Search API
  slug: search
  spec_type: OpenAPI
  url: https://app.zenserp.com/documentation
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zenserp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenserp secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zenserp
provider_slug: zenserp
scheme_count: 2
schemes:
- description: API key passed in the request header.
  in: header
  name: apiKeyHeader
  parameter: apikey
  sources:
  - openapi/zenserp-search-openapi.yml
  type: apiKey
- description: API key passed as a query parameter.
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/zenserp-search-openapi.yml
  type: apiKey
slug: zenserp-authentication
source_filename: zenserp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenserp-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key passed in the request header.\n  sources:\n  - openapi/zenserp-search-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key passed as a query parameter.\n  sources:\n  - openapi/zenserp-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/authentication/zenserp-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- SERP
- Search Engine Results
- Google Search
- Web Scraping
- SEO
- Image Search
- News Search
- Shopping Search
- Maps
- YouTube Search
- Bing
- Yandex
- DuckDuckGo
- Geolocation
- Keyword Research
---
