---
api_key_in:
- path
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Consensys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consensys secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Consensys
provider_slug: consensys
scheme_count: 1
schemes:
- description: Project/API key appended to the endpoint host as the final path segment (…/v3/<YOUR-API-KEY>). Applies across all supported networks.
  endpoint_example: https://mainnet.infura.io/v3/<YOUR-API-KEY>
  in: path
  management: https://app.infura.io/
  name: infuraApiKey
  parameter: v3/{API_KEY}
  type: apiKey
slug: consensys-authentication
source_filename: consensys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.infura.io/get-started/infura.md\ndocs: https://docs.metamask.io/services/\nsummary:\n  types: [apiKey]\n  api_key_in: [path]\n  oauth2_flows: []\nnote: >-\n  Infura (Consensys) authenticates JSON-RPC requests with an API key embedded in\n  the request URL path — e.g. https://mainnet.infura.io/v3/<YOUR-API-KEY>. API\n  keys are created and managed in the Infura dashboard (app.infura.io). There is\n  no OAuth surface for the JSON-RPC APIs; keys can be further restricted per\n  network/endpoint and optionally secured with an API key secret / allowlists.\nschemes:\n  - name: infuraApiKey\n    type: apiKey\n    in: path\n    parameter: v3/{API_KEY}\n    description: >-\n      Project/API key appended to the endpoint host as the final path segment\n      (…/v3/<YOUR-API-KEY>). Applies across all supported networks.\n    endpoint_example: https://mainnet.infura.io/v3/<YOUR-API-KEY>\n    management: https://app.infura.io/\n\
  key_hardening:\n  - API key secret (basic-auth style) can be required on requests.\n  - Allowlists: restrict a key by contract address, user-agent, origin, and request methods.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consensys/refs/heads/main/authentication/consensys-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Infrastructure
- Blockchain
- Ethereum
- Web3
- Developer Tools
- JSON-RPC
- Node Infrastructure
- Wallet
- Layer 2
---
