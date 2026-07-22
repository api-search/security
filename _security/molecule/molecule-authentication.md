---
api_key_in:
- header
auth_types:
- apiKey
- http
- custom
description: ''
kind: authentication
layout: security
method: searched
name: Molecule Authentication
name_suffix: Authentication
oauth_flows: []
overview: Molecule secures its APIs with apiKey, http, and custom across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Molecule
provider_slug: molecule
scheme_count: 4
schemes:
- in: header
  name: apiKey
  obtain: Contact the Molecule team via Discord with a use case.
  parameter_name: x-api-key
  required_for:
  - Data API
  - Tokenization API
  - Labs API queries
  - Labs API mutations
  sources:
  - docs:api-reference/api-reference.md
  - docs:api-reference/data-api.md
  type: apiKey
- in: header
  minted_by: generateServiceToken mutation (Privy session or wallet signature)
  name: serviceToken
  parameter_name: X-Service-Token
  required_for:
  - Labs API write mutations
  - Labs API legalAgreementTemplate query
  scope: Identifies the specific lab/dataroom the caller may write to.
  sources:
  - docs:api-reference/api-reference.md
  - docs:api-reference/labs-api.md
  type: apiKey
- description: HTTP 402 Payment Required flow (EIP-3009 transferWithAuthorization or Permit2, USDC on Base, Coinbase facilitator) fronting allow-listed Labs write mutations. Payment signature submitted in Payment-Signature / X-Payment / Payment header; gateway mints a short-lived (default 300s) scoped service token on success.
  name: x402-payment
  scheme: x402
  sources:
  - docs:api-reference/x402-gateway.md
  type: http
- description: File-level access control is enforced via Onchain-Verified Envelope Encryption (Lit Protocol retained for legacy files), not query authentication.
  name: onchain-access-control
  sources:
  - docs:core-concepts/data/data-privacy-and-access.md
  type: custom
slug: molecule-authentication
source_filename: molecule-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.molecule.xyz/api-reference/api-reference.md\ndocs: https://docs.molecule.xyz/api-reference/api-reference.md\nsummary:\n  types: [apiKey, http, custom]\n  api_key_in: [header]\n  notes: >-\n    All Molecule GraphQL APIs (Data, Tokenization, Labs) require an API key sent\n    in the x-api-key header. Labs API write mutations additionally require a\n    Service Token in the X-Service-Token header, scoped to a specific lab\n    (dataroom). Service tokens are minted via the generateServiceToken mutation,\n    which bootstraps from a Privy authenticated session or a wallet signature.\n    Autonomous agents without a long-lived service token can instead use the\n    x402 gateway, which mints a short-lived scoped service token after a\n    per-request USDC payment on Base is verified.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    required_for: [Data API, Tokenization\
  \ API, Labs API queries, Labs API mutations]\n    obtain: Contact the Molecule team via Discord with a use case.\n    sources: [docs:api-reference/api-reference.md, docs:api-reference/data-api.md]\n  - name: serviceToken\n    type: apiKey\n    in: header\n    parameter_name: X-Service-Token\n    required_for: [Labs API write mutations, \"Labs API legalAgreementTemplate query\"]\n    minted_by: generateServiceToken mutation (Privy session or wallet signature)\n    scope: Identifies the specific lab/dataroom the caller may write to.\n    sources: [docs:api-reference/api-reference.md, docs:api-reference/labs-api.md]\n  - name: x402-payment\n    type: http\n    scheme: x402\n    description: >-\n      HTTP 402 Payment Required flow (EIP-3009 transferWithAuthorization or\n      Permit2, USDC on Base, Coinbase facilitator) fronting allow-listed Labs\n      write mutations. Payment signature submitted in Payment-Signature /\n      X-Payment / Payment header; gateway mints a short-lived (default\
  \ 300s)\n      scoped service token on success.\n    sources: [docs:api-reference/x402-gateway.md]\n  - name: onchain-access-control\n    type: custom\n    description: >-\n      File-level access control is enforced via Onchain-Verified Envelope\n      Encryption (Lit Protocol retained for legacy files), not query\n      authentication.\n    sources: [docs:core-concepts/data/data-privacy-and-access.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/molecule/refs/heads/main/authentication/molecule-authentication.yml
summary_line: apiKey/http/custom · 4 schemes
tags:
- Company
- DeSci
- Decentralized Science
- Blockchain
- Web3
- GraphQL
- Intellectual Property
- IP-NFT
- Tokenization
- Life Sciences
- Biotech
- Research Funding
- AI Agents
- MCP
- x402
---
