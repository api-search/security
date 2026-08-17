---
api_key_in:
- query
api_specs:
- filename: talkwalker-search-openapi.yml
  format: yaml
  label: Talkwalker Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-search-openapi.yml
- filename: talkwalker-streaming-openapi.yml
  format: yaml
  label: Talkwalker Streaming API
  slug: streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-streaming-openapi.yml
- filename: talkwalker-histogram-openapi.yml
  format: yaml
  label: Talkwalker Histogram API
  slug: histogram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-histogram-openapi.yml
- filename: talkwalker-resources-openapi.yml
  format: yaml
  label: Talkwalker Resources API
  slug: resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-resources-openapi.yml
- filename: talkwalker-documents-openapi.yml
  format: yaml
  label: Talkwalker Document API
  slug: document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-documents-openapi.yml
- filename: talkwalker-image-openapi.yml
  format: yaml
  label: Talkwalker Image API
  slug: image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-image-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Talkwalker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talkwalker secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Talkwalker
provider_slug: talkwalker
scheme_count: 1
schemes:
- in: query
  name: apikeyAuth
  parameter: access_token
  sources:
  - openapi/talkwalker-documents-openapi.yml
  - openapi/talkwalker-histogram-openapi.yml
  - openapi/talkwalker-image-openapi.yml
  - openapi/talkwalker-resources-openapi.yml
  - openapi/talkwalker-search-openapi.yml
  - openapi/talkwalker-status-openapi.yml
  - openapi/talkwalker-streaming-openapi.yml
  type: apiKey
slug: talkwalker-authentication
source_filename: talkwalker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/talkwalker-documents-openapi.yml, openapi/talkwalker-histogram-openapi.yml,\n  openapi/talkwalker-image-openapi.yml, openapi/talkwalker-resources-openapi.yml, openapi/talkwalker-search-openapi.yml,\n  openapi/talkwalker-status-openapi.yml, openapi/talkwalker-streaming-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikeyAuth\n  type: apiKey\n  in: query\n  parameter: access_token\n  sources:\n  - openapi/talkwalker-documents-openapi.yml\n  - openapi/talkwalker-histogram-openapi.yml\n  - openapi/talkwalker-image-openapi.yml\n  - openapi/talkwalker-resources-openapi.yml\n  - openapi/talkwalker-search-openapi.yml\n  - openapi/talkwalker-status-openapi.yml\n  - openapi/talkwalker-streaming-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/authentication/talkwalker-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Social Media Analytics
- Social Listening
- Brand Monitoring
- Sentiment Analysis
- Media Monitoring
- Campaign Analytics
---
