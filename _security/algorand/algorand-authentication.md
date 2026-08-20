---
api_key_in:
- header
api_specs:
- filename: algorand-common-api-openapi.yml
  format: yaml
  label: Algorand common API
  slug: algorand-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-common-api-openapi.yml
- filename: algorand-data-api-openapi.yml
  format: yaml
  label: Algorand data API
  slug: algorand-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-data-api-openapi.yml
- filename: algorand-experimental-api-openapi.yml
  format: yaml
  label: Algorand experimental API
  slug: algorand-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-experimental-api-openapi.yml
- filename: algorand-key-api-openapi.yml
  format: yaml
  label: Algorand Key API
  slug: algorand-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-key-api-openapi.yml
- filename: algorand-lookup-api-openapi.yml
  format: yaml
  label: Algorand lookup API
  slug: algorand-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-lookup-api-openapi.yml
- filename: algorand-master-key-api-openapi.yml
  format: yaml
  label: Algorand Master Key API
  slug: algorand-master-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-master-key-api-openapi.yml
- filename: algorand-multisig-api-openapi.yml
  format: yaml
  label: Algorand Multisig API
  slug: algorand-multisig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-multisig-api-openapi.yml
- filename: algorand-nonparticipating-api-openapi.yml
  format: yaml
  label: Algorand nonparticipating API
  slug: algorand-nonparticipating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-nonparticipating-api-openapi.yml
- filename: algorand-participating-api-openapi.yml
  format: yaml
  label: Algorand participating API
  slug: algorand-participating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-participating-api-openapi.yml
- filename: algorand-private-api-openapi.yml
  format: yaml
  label: Algorand private API
  slug: algorand-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-private-api-openapi.yml
- filename: algorand-program-api-openapi.yml
  format: yaml
  label: Algorand Program API
  slug: algorand-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-program-api-openapi.yml
- filename: algorand-public-api-openapi.yml
  format: yaml
  label: Algorand public API
  slug: algorand-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-public-api-openapi.yml
- filename: algorand-search-api-openapi.yml
  format: yaml
  label: Algorand search API
  slug: algorand-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-search-api-openapi.yml
- filename: algorand-swagger-json-api-openapi.yml
  format: yaml
  label: Algorand Swagger.json API
  slug: algorand-swagger-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-swagger-json-api-openapi.yml
- filename: algorand-transaction-api-openapi.yml
  format: yaml
  label: Algorand Transaction API
  slug: algorand-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-transaction-api-openapi.yml
- filename: algorand-versions-api-openapi.yml
  format: yaml
  label: Algorand Versions API
  slug: algorand-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-versions-api-openapi.yml
- filename: algorand-wallet-api-openapi.yml
  format: yaml
  label: Algorand Wallet API
  slug: algorand-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-wallet-api-openapi.yml
- filename: algorand-wallets-api-openapi.yml
  format: yaml
  label: Algorand Wallets API
  slug: algorand-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/openapi/algorand-wallets-api-openapi.yml
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
- Proof of Stake
- DeFi
- Smart Contracts
---
