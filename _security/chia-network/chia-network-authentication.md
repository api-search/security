---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Chia Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chia Network secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chia Network
provider_slug: chia-network
scheme_count: 1
schemes:
- cert_files:
  - config/ssl/<service>/private_<service>.crt
  - config/ssl/<service>/private_<service>.key
  description: Chia RPC endpoints are secured with TLS mutual authentication using self-signed certificates. Each service (full_node, wallet, farmer, harvester, daemon, etc.) has its own private_ca / ssl cert + key pair generated on the node; clients must present the matching --cert and --key (and use --insecure against the self-signed CA). The RPC ports are intended to be bound to localhost and should NOT be exposed to the internet.
  name: mutualTLS
  sources:
  - docs.chia.net/rpc
  type: mutualTLS
slug: chia-network-authentication
source_filename: chia-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chia.net/rpc/\ndocs: https://docs.chia.net/rpc/\nsummary:\n  types: [mutualTLS]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      Chia RPC endpoints are secured with TLS mutual authentication using\n      self-signed certificates. Each service (full_node, wallet, farmer,\n      harvester, daemon, etc.) has its own private_ca / ssl cert + key pair\n      generated on the node; clients must present the matching --cert and --key\n      (and use --insecure against the self-signed CA). The RPC ports are intended\n      to be bound to localhost and should NOT be exposed to the internet.\n    sources: [docs.chia.net/rpc]\n    cert_files:\n      - config/ssl/<service>/private_<service>.crt\n      - config/ssl/<service>/private_<service>.key\nnotes: >-\n  There is no bearer/API-key or OAuth surface: authentication is the node\n  operator's own TLS cert\
  \ material. No published OpenAPI declares these schemes,\n  so this profile is searched from the RPC docs rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chia-network/refs/heads/main/authentication/chia-network-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Company
- Frontier Tech
- Blockchain
- Cryptocurrency
- Decentralized
- Web3
- Developer Tools
- Open Source
---
