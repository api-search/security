---
api_key_in:
- header
api_specs:
- filename: blockfrost-openapi.yaml
  format: yaml
  label: Blockfrost API
  slug: blockfrost
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/openapi/blockfrost-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Blockfrost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockfrost secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blockfrost
provider_slug: blockfrost
scheme_count: 1
schemes:
- description: 'There are multiple token types available based on network you choose

    when creating a Blockfrost a project, for a list of token types

    see available networks.'
  in: header
  name: project_id
  parameter: project_id
  sources:
  - openapi/blockfrost-openapi.yaml
  type: apiKey
slug: blockfrost-authentication
source_filename: blockfrost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blockfrost-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: project_id\n  type: apiKey\n  in: header\n  parameter: project_id\n  description: |-\n    There are multiple token types available based on network you choose\n    when creating a Blockfrost a project, for a list of token types\n    see available networks.\n  sources:\n  - openapi/blockfrost-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/authentication/blockfrost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
---
