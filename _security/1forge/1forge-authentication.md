---
api_key_in:
- query
api_specs:
- filename: 1forge-forex-data-api.yml
  format: yaml
  label: 1Forge Forex Data API
  slug: 1forge-forex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/openapi/1forge-forex-data-api.yml
- filename: 1forge-forex-stream-asyncapi.yml
  format: yaml
  label: 1Forge Forex Stream
  slug: 1forge-forex-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/asyncapi/1forge-forex-stream-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 1Forge Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Forge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 1Forge
provider_slug: 1forge
scheme_count: 1
schemes:
- description: '1Forge requires an API key passed as the `api_key` query parameter on every

    request. Obtain a key at https://1forge.com.'
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/1forge-forex-data-api.yml
  type: apiKey
slug: 1forge-authentication
source_filename: 1forge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/1forge-forex-data-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: |-\n    1Forge requires an API key passed as the `api_key` query parameter on every\n    request. Obtain a key at https://1forge.com.\n  sources:\n  - openapi/1forge-forex-data-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/authentication/1forge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Currency Exchange
- Forex
- Cryptocurrency
- Market Data
- Financial Data
- Real-Time Data
---
