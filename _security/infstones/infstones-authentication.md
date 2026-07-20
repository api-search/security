---
api_key_in:
- path
api_specs:
- filename: infstones-bnb-chain-openapi.json
  format: json
  label: InfStones RPC API
  slug: infstones-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infstones/refs/heads/main/openapi/infstones-bnb-chain-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Infstones Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfStones secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InfStones
provider_slug: infstones
scheme_count: 1
schemes:
- description: Per-project API key issued from the InfStones console, placed in the endpoint path (/{project_id}). Scopes RPC requests to the owning project/plan.
  in: path
  name: projectIdPathKey
  parameter: project_id
  sources:
  - openapi/infstones-bnb-chain-openapi.json
  type: apiKey
slug: infstones-authentication
source_filename: infstones-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.infstones.com/reference\ndocs: https://docs.infstones.com/reference/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [path]\n  note: >-\n    InfStones RPC access is authenticated by a per-project API key (project_id)\n    carried in the request path segment of the endpoint URL, e.g.\n    https://api.infstones.com/bsc/mainnet/{project_id}. The key is issued from the\n    InfStones developer console (https://app.infstones.com/api). The provider's\n    ReadMe-generated OpenAPI declares an empty security requirement, but the\n    project_id path parameter is the effective credential. No OAuth2 or OIDC flow\n    is exposed for RPC access.\nschemes:\n- name: projectIdPathKey\n  type: apiKey\n  in: path\n  parameter: project_id\n  description: >-\n    Per-project API key issued from the InfStones console, placed in the endpoint\n    path (/{project_id}). Scopes RPC requests to the owning project/plan.\n  sources:\n\
  \  - openapi/infstones-bnb-chain-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infstones/refs/heads/main/authentication/infstones-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Node Infrastructure
- Staking
- Web3
- JSON-RPC
- RPC
- Ethereum
- BNB Chain
- Cosmos
- Cryptocurrency
- API
---
