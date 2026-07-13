---
api_key_in:
- header
api_specs:
- filename: introduction
  format: yaml
  label: X2Y2 OpenAPI
  slug: x2y2-openapi
  spec_type: OpenAPI
  url: https://x2y2.readme.io/reference/introduction
- filename: introduction
  format: yaml
  label: X2Y2 Fi API
  slug: x2y2-fi-api
  spec_type: OpenAPI
  url: https://x2y2.readme.io/reference/introduction
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: X2Y2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: X2Y2 secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: X2Y2
provider_slug: x2y2
scheme_count: 3
schemes:
- in: header
  name: sec0
  parameter: X-API-KEY
  sources:
  - openapi/x2y2-fi-api.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/x2y2-openapi.json
  type: apiKey
- in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/x2y2-post-apis.json
  type: apiKey
slug: x2y2-authentication
source_filename: x2y2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/x2y2-fi-api.json, openapi/x2y2-openapi.json, openapi/x2y2-post-apis.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/x2y2-fi-api.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/x2y2-openapi.json\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/x2y2-post-apis.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x2y2/refs/heads/main/authentication/x2y2-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- NFT
- Ethereum
- Marketplace
- Blockchain
- Web3
- Collectibles
- Trading
---
