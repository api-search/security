---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: DEGIRO Trading API
  slug: degiro-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/degiro/refs/heads/main/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Degiro Authentication
name_suffix: Authentication
oauth_flows: []
overview: DEGIRO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DEGIRO
provider_slug: degiro
scheme_count: 2
schemes:
- in: query
  name: SessionIdAuth
  parameter: sessionId
  sources:
  - openapi/degiro-openapi.yml
  type: apiKey
- in: query
  name: IntAccountAuth
  parameter: intAccount
  sources:
  - openapi/degiro-openapi.yml
  type: apiKey
slug: degiro-authentication
source_filename: degiro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/degiro-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: SessionIdAuth\n  type: apiKey\n  in: query\n  parameter: sessionId\n  sources:\n  - openapi/degiro-openapi.yml\n- name: IntAccountAuth\n  type: apiKey\n  in: query\n  parameter: intAccount\n  sources:\n  - openapi/degiro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/degiro/refs/heads/main/authentication/degiro-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Trading
- Brokerage
- Stocks
- ETFs
- Portfolio
- Market Data
- Finance
---
