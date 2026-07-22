---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Morpho Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Morpho Labs secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Morpho Labs
provider_slug: morpho-labs
scheme_count: 0
schemes: []
slug: morpho-labs-authentication
source_filename: morpho-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.morpho.org/tools/offchain/api/get-started/\ndocs: https://docs.morpho.org/tools/offchain/api/get-started/\napi: Morpho API (GraphQL)\nsummary:\n  types: [none]\n  auth_required: false\n  notes: >-\n    The Morpho public GraphQL API requires no API key, token, or OAuth flow —\n    read access to markets, vaults, positions, and onchain/offchain data is\n    open. Access is governed by rate limiting (750 req/min) and query-complexity\n    limits rather than authentication. Onchain write operations are executed by\n    the caller's own EVM wallet via the SDKs (transaction signing happens\n    client-side against the smart contracts, not against an authenticated API).\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morpho-labs/refs/heads/main/authentication/morpho-labs-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- DeFi
- Lending
- Blockchain
- Ethereum
- GraphQL
- Onchain Data
- Financial Services
- Web3
- Crypto
---
