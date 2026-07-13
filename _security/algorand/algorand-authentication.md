---
api_key_in:
- header
api_specs:
- filename: algod.oas3.yml
  format: yaml
  label: Algorand Algod REST API
  slug: algorand-algod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/algorand/go-algorand/master/daemon/algod/api/algod.oas3.yml
- filename: indexer.oas3.yml
  format: yaml
  label: Algorand Indexer REST API
  slug: algorand-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/algorand/indexer/main/api/indexer.oas3.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Algorand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Algorand secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Algorand
provider_slug: algorand
scheme_count: 2
schemes:
- description: Generated header parameter. This token can be generated using the Goal command line tool. Example value ='b7e384d0317b8050ce45900a94a1931e28540e1f69b2d242b424659c341b4697'
  in: header
  name: api_key
  parameter: X-Algo-API-Token
  sources:
  - openapi/algorand-algod-openapi.json
  type: apiKey
- description: 'Generated header parameter. This value can be found in `/kmd/data/dir/kmd.token`. Example value: ''330b2e4fc9b20f4f89812cf87f1dabeb716d23e3f11aec97a61ff5f750563b78'''
  in: header
  name: api_key
  parameter: X-KMD-API-Token
  sources:
  - openapi/algorand-kmd-openapi.json
  type: apiKey
slug: algorand-authentication
source_filename: algorand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/algorand-algod-openapi.json, openapi/algorand-kmd-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Algo-API-Token\n  description: Generated header parameter. This token can be generated using the Goal command\n    line tool. Example value ='b7e384d0317b8050ce45900a94a1931e28540e1f69b2d242b424659c341b4697'\n  sources:\n  - openapi/algorand-algod-openapi.json\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-KMD-API-Token\n  description: 'Generated header parameter. This value can be found in `/kmd/data/dir/kmd.token`.\n    Example value: ''330b2e4fc9b20f4f89812cf87f1dabeb716d23e3f11aec97a61ff5f750563b78'''\n  sources:\n  - openapi/algorand-kmd-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/authentication/algorand-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Blockchain
- Cryptocurrency
- Proof-of-Stake
- DeFi
- Smart Contracts
---
