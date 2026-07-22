---
api_key_in: []
api_specs:
- filename: tendermint-rpc-openapi-original.yml
  format: yaml
  label: Tendermint RPC
  slug: tendermint-rpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tendermint/refs/heads/main/openapi/tendermint-rpc-openapi-original.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Tendermint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tendermint declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Tendermint
provider_slug: tendermint
scheme_count: 0
schemes: []
slug: tendermint-authentication
source_filename: tendermint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tendermint-rpc-openapi-original.yml\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: none\nschemes: []\nnotes: >-\n  The Tendermint RPC OpenAPI declares no securitySchemes. Node RPC is\n  unauthenticated by design — access control is a deployment concern (bind\n  address, reverse proxy, firewall, allowlist). The \"Unsafe\" tagged operations\n  (dial_seeds, dial_peers) are additionally gated behind an unsafe-RPC node\n  flag rather than any token. Operators typically restrict RPC exposure at the\n  network layer; there is no OAuth, API key, or bearer token surface to\n  document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tendermint/refs/heads/main/authentication/tendermint-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Infrastructure
- Blockchain
- Consensus
- Cosmos
- Web3
- JSON-RPC
- Node
---
