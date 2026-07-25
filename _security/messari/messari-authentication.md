---
api_key_in:
- header
api_specs:
- filename: messari-ai-api-openapi.yml
  format: yaml
  label: Messari AI API
  slug: messari-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-ai-api-openapi.yml
- filename: messari-assets-api-openapi.yml
  format: yaml
  label: Messari Assets API
  slug: messari-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-assets-api-openapi.yml
- filename: messari-datasets-api-openapi.yml
  format: yaml
  label: Messari Datasets API
  slug: messari-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-datasets-api-openapi.yml
- filename: messari-exchanges-api-openapi.yml
  format: yaml
  label: Messari Exchanges API
  slug: messari-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-exchanges-api-openapi.yml
- filename: messari-markets-api-openapi.yml
  format: yaml
  label: Messari Markets API
  slug: messari-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-markets-api-openapi.yml
- filename: messari-monitoring-api-openapi.yml
  format: yaml
  label: Messari Monitoring API
  slug: messari-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-monitoring-api-openapi.yml
- filename: messari-networks-api-openapi.yml
  format: yaml
  label: Messari Networks API
  slug: messari-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-networks-api-openapi.yml
- filename: messari-news-api-openapi.yml
  format: yaml
  label: Messari News API
  slug: messari-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-news-api-openapi.yml
- filename: messari-protocols-api-openapi.yml
  format: yaml
  label: Messari Protocols API
  slug: messari-protocols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-protocols-api-openapi.yml
- filename: messari-research-api-openapi.yml
  format: yaml
  label: Messari Research API
  slug: messari-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-research-api-openapi.yml
- filename: messari-token-unlocks-api-openapi.yml
  format: yaml
  label: Messari Token Unlocks API
  slug: messari-token-unlocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-token-unlocks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Messari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Messari secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Messari
provider_slug: messari
scheme_count: 1
schemes:
- description: Messari API key
  in: header
  name: apiKeyAuth
  parameter: x-messari-api-key
  sources:
  - openapi/messari-openapi.yml
  type: apiKey
slug: messari-authentication
source_filename: messari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/messari-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-messari-api-key\n  description: Messari API key\n  sources:\n  - openapi/messari-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/authentication/messari-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- Research
- Analytics
- Asset Data
- Fundamentals
- News
- Token Unlocks
---
