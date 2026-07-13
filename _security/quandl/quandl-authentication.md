---
api_key_in:
- header
- query
api_specs:
- filename: nasdaq-data-link-timeseries-openapi.yml
  format: yaml
  label: Nasdaq Data Link REST API (Time-Series)
  slug: nasdaq-data-link-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandl/refs/heads/main/openapi/nasdaq-data-link-timeseries-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quandl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quandl (Nasdaq Data Link) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quandl (Nasdaq Data Link)
provider_slug: quandl
scheme_count: 2
schemes:
- description: Nasdaq Data Link API key passed as query parameter
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/nasdaq-data-link-timeseries-openapi.yml
  type: apiKey
- description: Nasdaq Data Link API key passed as header
  in: header
  name: apiKeyHeader
  parameter: X-Api-Token
  sources:
  - openapi/nasdaq-data-link-timeseries-openapi.yml
  type: apiKey
slug: quandl-authentication
source_filename: quandl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nasdaq-data-link-timeseries-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Nasdaq Data Link API key passed as query parameter\n  sources:\n  - openapi/nasdaq-data-link-timeseries-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Token\n  description: Nasdaq Data Link API key passed as header\n  sources:\n  - openapi/nasdaq-data-link-timeseries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandl/refs/heads/main/authentication/quandl-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Finance
- Market Data
- Economic Data
- Time Series
- Streaming
---
