---
api_key_in: []
auth_types:
- apiKey
- web3-wallet
description: ''
kind: authentication
layout: security
method: searched
name: Toucan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toucan secures its APIs with apiKey and web3-wallet across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Toucan
provider_slug: toucan
scheme_count: 2
schemes:
- description: 'The Graph gateway API key embedded in the subgraph endpoint URL: https://gateway-arbitrum.network.thegraph.com/api/[api-key]/subgraphs/id/<subgraph-id>'
  docs: https://thegraph.com/studio/apikeys/
  in: path
  name: graphApiKey
  surfaces:
  - subgraphs
  type: apiKey
- description: EVM wallet signer/provider (ethers.js ^5.6.4 recommended; wagmi <1.0 supported) used by the toucan-sdk ToucanClient for contract reads and writes on Celo, Polygon, and Base networks.
  docs: https://docs.toucan.earth/developers/sdk/quickstart
  name: walletSigner
  surfaces:
  - smart-contracts
  - sdk
  type: web3-wallet
slug: toucan-authentication
source_filename: toucan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.toucan.earth/developers/subgraph\ndocs: https://docs.toucan.earth/developers/sdk/quickstart\nsummary:\n  types: [apiKey, web3-wallet]\n  notes: >-\n    Toucan has no proprietary REST auth. Its two developer surfaces authenticate\n    differently: (1) the Toucan Subgraphs are served through The Graph's gateway\n    and require a Graph API key in the request path, generated at\n    https://thegraph.com/studio/apikeys/ after creating an account; (2) smart\n    contract interactions (directly or via the toucan-sdk ToucanClient) are\n    authorized by an EVM wallet signer (e.g. ethers.js Signer) — a provider alone\n    gives read-only access, a signer enables writes.\nschemes:\n  - name: graphApiKey\n    type: apiKey\n    in: path\n    description: >-\n      The Graph gateway API key embedded in the subgraph endpoint URL:\n      https://gateway-arbitrum.network.thegraph.com/api/[api-key]/subgraphs/id/<subgraph-id>\n\
  \    docs: https://thegraph.com/studio/apikeys/\n    surfaces: [subgraphs]\n  - name: walletSigner\n    type: web3-wallet\n    description: >-\n      EVM wallet signer/provider (ethers.js ^5.6.4 recommended; wagmi <1.0\n      supported) used by the toucan-sdk ToucanClient for contract reads and\n      writes on Celo, Polygon, and Base networks.\n    docs: https://docs.toucan.earth/developers/sdk/quickstart\n    surfaces: [smart-contracts, sdk]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toucan/refs/heads/main/authentication/toucan-authentication.yml
summary_line: apiKey/web3-wallet · 2 schemes
tags:
- Company
- Planetary Health
- Carbon Credits
- Climate
- Web3
- Carbon Markets
- Tokenization
- GraphQL
- Biochar
---
