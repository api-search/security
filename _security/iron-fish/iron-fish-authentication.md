---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Iron Fish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iron Fish secures its APIs with none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Iron Fish
provider_slug: iron-fish
scheme_count: 2
schemes:
- applies_to: read endpoints
  evidence: GET /blocks and GET /health return 200 without credentials.
  name: none
  surface: Public REST API (api.ironfish.network)
  type: none
- name: node-local
  note: No token is required by default; the operator controls exposure via rpcHttpHost / rpcTcpHost binding. TLS + encryption are available on the multisig broker server (added in ironfish 2.8.0).
  surface: Node RPC (TCP/IPC/HTTP, default TCP port 8020)
  type: none
slug: iron-fish-authentication
source_filename: iron-fish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://ironfish.network/developers/documentation/integration_rpc + live probe of https://api.ironfish.network\ndocs: https://ironfish.network/developers/documentation/integration_rpc\nsummary:\n  types: [none]\n  note: >-\n    Iron Fish is a self-hosted node model. The public REST API at\n    api.ironfish.network serves read endpoints (e.g. /blocks, /health) with no\n    authentication. The node RPC server is bound locally by the operator; access\n    control is a matter of network exposure (host/port binding and optional TLS\n    on the multisig broker) rather than an API-key or OAuth scheme.\nschemes:\n- name: none\n  surface: Public REST API (api.ironfish.network)\n  type: none\n  applies_to: read endpoints\n  evidence: GET /blocks and GET /health return 200 without credentials.\n- name: node-local\n  surface: Node RPC (TCP/IPC/HTTP, default TCP port 8020)\n  type: none\n  note: >-\n    No token is required by default;\
  \ the operator controls exposure via\n    rpcHttpHost / rpcTcpHost binding. TLS + encryption are available on the\n    multisig broker server (added in ironfish 2.8.0).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iron-fish/refs/heads/main/authentication/iron-fish-authentication.yml
summary_line: none · 2 schemes
tags:
- Blockchain
- Cryptocurrency
- Privacy
- Zero Knowledge
- Layer 1
- Web3
- RPC
- Wallet
---
