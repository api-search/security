---
api_key_in:
- header
- query
api_specs:
- filename: finnhub-asyncapi.yml
  format: yaml
  label: Finnhub
  slug: finnhub
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/finnhub/refs/heads/main/asyncapi/finnhub-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Finnhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finnhub secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finnhub
provider_slug: finnhub
scheme_count: 2
schemes:
- in: query
  name: tokenQuery
  parameter: token
  sources:
  - openapi/finnhub-openapi.yml
  type: apiKey
- in: header
  name: tokenHeader
  parameter: X-Finnhub-Token
  sources:
  - openapi/finnhub-openapi.yml
  type: apiKey
slug: finnhub-authentication
source_filename: finnhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/finnhub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: tokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/finnhub-openapi.yml\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Finnhub-Token\n  sources:\n  - openapi/finnhub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finnhub/refs/heads/main/authentication/finnhub-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Financial
- Market Data
- Stocks
---
