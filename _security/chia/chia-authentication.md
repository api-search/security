---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Chia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chia secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chia
provider_slug: chia
scheme_count: 1
schemes:
- description: Every Chia JSON-RPC service (full node, wallet, farmer, harvester, DataLayer, DID, NFT, offers, DAO, VC, simulator, daemon) authenticates callers with a private/self node TLS client certificate + key generated into the Chia SSL directory (~/.chia/mainnet/config/ssl/). The client must present the matching private_crt/private_key pair; there are no API keys, bearer tokens, or OAuth. Endpoints are self-hosted and default to loopback, so access control is the local node's certificate material.
  name: mutualTLS
  sources:
  - docs.chia.net/rpc/
  type: mutualTLS
slug: chia-authentication
source_filename: chia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chia.net/rpc/\ndocs: https://docs.chia.net/rpc/\nsummary:\n  types: [mutualTLS]\n  transport: HTTPS (POST JSON) or WebSocket, localhost per-service ports\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      Every Chia JSON-RPC service (full node, wallet, farmer, harvester,\n      DataLayer, DID, NFT, offers, DAO, VC, simulator, daemon) authenticates\n      callers with a private/self node TLS client certificate + key generated\n      into the Chia SSL directory (~/.chia/mainnet/config/ssl/). The client must\n      present the matching private_crt/private_key pair; there are no API keys,\n      bearer tokens, or OAuth. Endpoints are self-hosted and default to\n      loopback, so access control is the local node's certificate material.\n    sources: [docs.chia.net/rpc/]\nnotes: >-\n  DataLayer additionally supports an HTTP/S data-propagation server;\
  \ RPC control\n  planes remain mutual-TLS. Derived-from-OpenAPI is not possible (Chia publishes\n  no OpenAPI); this profile is captured from the published RPC reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chia/refs/heads/main/authentication/chia-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Company
- Blockchain
- Cryptocurrency
- Web3
- Decentralized
- JSON-RPC
- Developer Tools
- Open Source
---
