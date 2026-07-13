---
api_key_in:
- header
api_specs:
- filename: moralis-evm-api-openapi.json
  format: json
  label: Moralis EVM API
  slug: evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moralis/refs/heads/main/openapi/moralis-evm-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Moralis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moralis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moralis
provider_slug: moralis
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/moralis-evm-api-openapi.json
  type: apiKey
slug: moralis-authentication
source_filename: moralis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moralis-evm-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/moralis-evm-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moralis/refs/heads/main/authentication/moralis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Blockchain
- Data API
- Streams
- Indexing
---
