---
api_key_in:
- query
api_specs:
- filename: openapi.json
  format: json
  label: PolygonScan API
  slug: polygonscan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygonscan/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Polygonscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: PolygonScan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PolygonScan
provider_slug: polygonscan
scheme_count: 1
schemes:
- description: API key obtained from https://polygonscan.com/myapikey
  in: query
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/openapi.json
  type: apiKey
slug: polygonscan-authentication
source_filename: polygonscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key obtained from https://polygonscan.com/myapikey\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygonscan/refs/heads/main/authentication/polygonscan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Polygon
- Explorer
- Web3
- EVM
- Smart Contracts
- DeFi
- Cryptocurrency
---
