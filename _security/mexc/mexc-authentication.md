---
api_key_in:
- header
api_specs:
- filename: mexc-spot-rest-api-openapi.json
  format: json
  label: MEXC Spot REST API
  slug: spot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-spot-rest-api-openapi.json
- filename: mexc-futures-rest-api-openapi.json
  format: json
  label: MEXC Futures REST API
  slug: futures-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-futures-rest-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mexc Authentication
name_suffix: Authentication
oauth_flows: []
overview: MEXC secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MEXC
provider_slug: mexc
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-MEXC-APIKEY
  sources:
  - openapi/mexc-futures-rest-api-openapi.json
  - openapi/mexc-spot-rest-api-openapi.json
  type: apiKey
slug: mexc-authentication
source_filename: mexc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mexc-futures-rest-api-openapi.json, openapi/mexc-spot-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-MEXC-APIKEY\n  sources:\n  - openapi/mexc-futures-rest-api-openapi.json\n  - openapi/mexc-spot-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/authentication/mexc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Exchange
- Trading
- Futures
- Market Data
- Finance
- Blockchain
---
