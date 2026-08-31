---
api_key_in:
- query
api_specs:
- filename: talkwalker-image-api-api-openapi.yml
  format: yaml
  label: Talkwalker Image API
  slug: talkwalker-image-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-image-api-api-openapi.yml
- filename: talkwalker-modify-documents-api-api-openapi.yml
  format: yaml
  label: Talkwalker Modify documents API
  slug: talkwalker-modify-documents-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-modify-documents-api-api-openapi.yml
- filename: talkwalker-resources-api-api-openapi.yml
  format: yaml
  label: Talkwalker Resources API
  slug: talkwalker-resources-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-resources-api-api-openapi.yml
- filename: talkwalker-search-api-api-openapi.yml
  format: yaml
  label: Talkwalker Search API
  slug: talkwalker-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-search-api-api-openapi.yml
- filename: talkwalker-search-api-histogram-api-api-openapi.yml
  format: yaml
  label: Talkwalker Search API > Histogram API
  slug: talkwalker-search-api-histogram-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-search-api-histogram-api-api-openapi.yml
- filename: talkwalker-source-panels-api-api-openapi.yml
  format: yaml
  label: Talkwalker Source panels API
  slug: talkwalker-source-panels-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-source-panels-api-api-openapi.yml
- filename: talkwalker-status-api-api-openapi.yml
  format: yaml
  label: Talkwalker Status API
  slug: talkwalker-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-status-api-api-openapi.yml
- filename: talkwalker-streaming-api-api-openapi.yml
  format: yaml
  label: Talkwalker Streaming API
  slug: talkwalker-streaming-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-streaming-api-api-openapi.yml
- filename: talkwalker-streaming-api-collector-api-api-openapi.yml
  format: yaml
  label: Talkwalker Streaming API > Collector API
  slug: talkwalker-streaming-api-collector-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-streaming-api-collector-api-api-openapi.yml
- filename: talkwalker-streaming-api-task-api-api-openapi.yml
  format: yaml
  label: Talkwalker Streaming API > Task API
  slug: talkwalker-streaming-api-task-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-streaming-api-task-api-api-openapi.yml
- filename: talkwalker-summary-api-api-openapi.yml
  format: yaml
  label: Talkwalker Summary API
  slug: talkwalker-summary-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-summary-api-api-openapi.yml
- filename: talkwalker-topic-api-api-openapi.yml
  format: yaml
  label: Talkwalker Topic API
  slug: talkwalker-topic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/openapi/talkwalker-topic-api-api-openapi.yml
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
