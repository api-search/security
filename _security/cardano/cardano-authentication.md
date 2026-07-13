---
api_key_in:
- header
api_specs:
- filename: blockfrost-cardano-api-openapi.yml
  format: yaml
  label: Blockfrost Cardano API
  slug: blockfrost-cardano-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardano/refs/heads/main/openapi/blockfrost-cardano-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cardano Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cardano secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cardano
provider_slug: cardano
scheme_count: 1
schemes:
- description: 'There are multiple token types available based on network you choose

    when creating a Blockfrost a project, for a list of token types

    see available networks.'
  in: header
  name: project_id
  parameter: project_id
  sources:
  - openapi/blockfrost-cardano-api-openapi.yml
  type: apiKey
slug: cardano-authentication
source_filename: cardano-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blockfrost-cardano-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: project_id\n  type: apiKey\n  in: header\n  parameter: project_id\n  description: |-\n    There are multiple token types available based on network you choose\n    when creating a Blockfrost a project, for a list of token types\n    see available networks.\n  sources:\n  - openapi/blockfrost-cardano-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardano/refs/heads/main/authentication/cardano-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- Proof-of-Stake
- Smart Contracts
- Web3
---
