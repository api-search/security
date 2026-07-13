---
api_key_in:
- header
- query
api_specs:
- filename: rainbow-ai-nowcast-openapi.yml
  format: yaml
  label: Rainbow.AI Nowcast API
  slug: rainbow-ai-nowcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/openapi/rainbow-ai-nowcast-openapi.yml
- filename: rainbow-ai-tiles-openapi.yml
  format: yaml
  label: Rainbow.AI Tiles API
  slug: rainbow-ai-tiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/openapi/rainbow-ai-tiles-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rainbow Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainbow.AI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rainbow.AI
provider_slug: rainbow-ai
scheme_count: 2
schemes:
- description: API key passed in the Ocp-Apim-Subscription-Key header
  in: header
  name: ApiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/rainbow-ai-nowcast-openapi.yml
  - openapi/rainbow-ai-tiles-openapi.yml
  type: apiKey
- description: API key passed as a token query parameter
  in: query
  name: ApiKeyQuery
  parameter: token
  sources:
  - openapi/rainbow-ai-nowcast-openapi.yml
  - openapi/rainbow-ai-tiles-openapi.yml
  type: apiKey
slug: rainbow-ai-authentication
source_filename: rainbow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rainbow-ai-nowcast-openapi.yml, openapi/rainbow-ai-tiles-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: API key passed in the Ocp-Apim-Subscription-Key header\n  sources:\n  - openapi/rainbow-ai-nowcast-openapi.yml\n  - openapi/rainbow-ai-tiles-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: API key passed as a token query parameter\n  sources:\n  - openapi/rainbow-ai-nowcast-openapi.yml\n  - openapi/rainbow-ai-tiles-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/authentication/rainbow-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Weather
- Precipitation
- Forecasting
- Nowcast
- Radar
- Tiles
- Geospatial
---
