---
api_key_in:
- header
api_specs:
- filename: api
  format: yaml
  label: Avalanche Data API (Glacier)
  slug: avalanche-data-api-glacier
  spec_type: OpenAPI
  url: https://glacier-api.avax.network/api
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Avalanche Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avalanche secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avalanche
provider_slug: avalanche
scheme_count: 1
schemes:
- description: Api keys provide higher access to rate limits. To obtain an api key, sign up for an account at  https://build.avax.network/console/utilities/data-api-keys.
  in: header
  name: apiKey
  parameter: x-glacier-api-key
  sources:
  - openapi/data-api.json
  type: apiKey
slug: avalanche-authentication
source_filename: avalanche-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/data-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-glacier-api-key\n  description: Api keys provide higher access to rate limits. To obtain an api key, sign up\n    for an account at  https://build.avax.network/console/utilities/data-api-keys.\n  sources:\n  - openapi/data-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalanche/refs/heads/main/authentication/avalanche-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Web3
- Avalanche
- NFT
- DeFi
- Cross-Chain
---
