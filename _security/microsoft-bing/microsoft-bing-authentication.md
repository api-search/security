---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-bing-autosuggest-api-openapi.yml
  format: yaml
  label: Microsoft Bing Autosuggest API
  slug: microsoft-bing-autosuggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-autosuggest-api-openapi.yml
- filename: microsoft-bing-custom-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Custom Search API
  slug: microsoft-bing-custom-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-custom-search-api-openapi.yml
- filename: microsoft-bing-entity-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Entity Search API
  slug: microsoft-bing-entity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-entity-search-api-openapi.yml
- filename: microsoft-bing-image-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Image Search API
  slug: microsoft-bing-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-image-search-api-openapi.yml
- filename: microsoft-bing-news-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing News Search API
  slug: microsoft-bing-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-news-search-api-openapi.yml
- filename: microsoft-bing-spell-check-api-openapi.yml
  format: yaml
  label: Microsoft Bing Spell Check API
  slug: microsoft-bing-spell-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-spell-check-api-openapi.yml
- filename: microsoft-bing-video-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Video Search API
  slug: microsoft-bing-video-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-video-search-api-openapi.yml
- filename: microsoft-bing-visual-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Visual search API
  slug: microsoft-bing-visual-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-visual-search-api-openapi.yml
- filename: microsoft-bing-web-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Web Search API
  slug: microsoft-bing-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-web-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Bing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bing secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Bing
provider_slug: microsoft-bing
scheme_count: 1
schemes:
- in: header
  name: subscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/microsoft-bing-openapi.yml
  type: apiKey
slug: microsoft-bing-authentication
source_filename: microsoft-bing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-bing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/microsoft-bing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/authentication/microsoft-bing-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- Web Search
- Image
- Video
- News
- Azure AI
- Autosuggest
- Visual Search
---
