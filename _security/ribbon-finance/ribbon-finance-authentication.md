---
api_key_in:
- header
api_specs:
- filename: aevo-public-rest-api.json
  format: json
  label: Aevo Exchange Public REST API
  slug: aevo-exchange-public-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/aevo-public-rest-api.json
- filename: aevo-private-rest-api.json
  format: json
  label: Aevo Exchange Private REST API
  slug: aevo-exchange-private-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/aevo-private-rest-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ribbon Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ribbon Finance secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ribbon Finance
provider_slug: ribbon-finance
scheme_count: 2
schemes:
- description: API key obtained from Aevo account settings
  in: header
  name: AevoKey
  parameter: AEVO-KEY
  sources:
  - openapi/aevo-private-rest-api.json
  type: apiKey
- description: API secret obtained from Aevo account settings
  in: header
  name: AevoSecret
  parameter: AEVO-SECRET
  sources:
  - openapi/aevo-private-rest-api.json
  type: apiKey
slug: ribbon-finance-authentication
source_filename: ribbon-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aevo-private-rest-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AevoKey\n  type: apiKey\n  in: header\n  parameter: AEVO-KEY\n  description: API key obtained from Aevo account settings\n  sources:\n  - openapi/aevo-private-rest-api.json\n- name: AevoSecret\n  type: apiKey\n  in: header\n  parameter: AEVO-SECRET\n  description: API secret obtained from Aevo account settings\n  sources:\n  - openapi/aevo-private-rest-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/authentication/ribbon-finance-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- DeFi
- Finance
- Options
- Structured Products
- Ethereum
- Layer 2
- Vaults
- Perpetuals
- Yield
---
