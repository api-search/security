---
api_key_in:
- header
- query
api_specs:
- filename: youscan-data-import-api-openapi.yml
  format: yaml
  label: YouScan Data Import API
  slug: youscan-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-data-import-api-openapi.yml
- filename: youscan-history-api-openapi.yml
  format: yaml
  label: YouScan History API
  slug: youscan-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-history-api-openapi.yml
- filename: youscan-mentions-api-openapi.yml
  format: yaml
  label: YouScan Mentions API
  slug: youscan-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-mentions-api-openapi.yml
- filename: youscan-spaces-api-openapi.yml
  format: yaml
  label: YouScan Spaces API
  slug: youscan-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-spaces-api-openapi.yml
- filename: youscan-statistics-api-openapi.yml
  format: yaml
  label: YouScan Statistics API
  slug: youscan-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-statistics-api-openapi.yml
- filename: youscan-tags-api-openapi.yml
  format: yaml
  label: YouScan Tags API
  slug: youscan-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-tags-api-openapi.yml
- filename: youscan-topics-api-openapi.yml
  format: yaml
  label: YouScan Topics API
  slug: youscan-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-topics-api-openapi.yml
- filename: youscan-webhook-api-openapi.yml
  format: yaml
  label: YouScan Webhook API
  slug: youscan-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/openapi/youscan-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Youscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: YouScan secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: YouScan
provider_slug: youscan
scheme_count: 2
schemes:
- description: API key authentication. The recommended way to authenticate requests.
  in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/youscan-openapi.yaml
  type: apiKey
- description: API key as a query parameter. For testing purposes only.
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/youscan-openapi.yaml
  type: apiKey
slug: youscan-authentication
source_filename: youscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/youscan-openapi.yaml\ndocs: https://help.youscan.io/en/articles/2754452-how-to-use-youscan-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key authentication. The recommended way to authenticate requests.\n  sources:\n  - openapi/youscan-openapi.yaml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key as a query parameter. For testing purposes only.\n  sources:\n  - openapi/youscan-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youscan/refs/heads/main/authentication/youscan-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Social Media Listening
- Social Intelligence
- Consumer Insights
- Sentiment Analysis
- Media Monitoring
- Analytics
- Artificial Intelligence
---
