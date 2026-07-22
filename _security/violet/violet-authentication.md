---
api_key_in: []
auth_types:
- oauth2
- onchain-registry
description: ''
kind: authentication
layout: security
method: searched
name: Violet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Violet secures its APIs with oauth2 and onchain-registry across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Violet
provider_slug: violet
scheme_count: 2
schemes:
- description: An Ethereum Access Token is a signed compliance assertion issued by the Violet system (off-chain) and verified by the Violet Verifier smart contract (on-chain). It carries no direct PII; it only attests that a wallet address has enrolled and satisfies the compliance requirements of the integrating dApp. EATs are fully OAuth 2.0 compliant.
  flow: authorizationCode
  name: EthereumAccessToken
  source: https://docs.violet.co/for-developers/core-concepts/ethereum-access-token
  token_format: EIP-712 signed message
  type: oauth2
  verifier_contract: '0xe8F42626ba40be4478B4B13566E9B26faff33663'
- description: An on-chain registry mapping a wallet address to compliance statuses. Any integrating dApp can query compliance status directly on-chain without a round-trip to Violet; only Violet can modify entries. Used as an alternative integration path to the EAT flow.
  name: VioletIDRegistry
  registry_contract: '0xfFcDa323597A90af8F7A0eCBE4ef14e9b30e4a9e'
  source: https://docs.violet.co/for-developers/core-concepts/violetid-registry
  type: onchain-registry
slug: violet-authentication
source_filename: violet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.violet.co/for-developers/core-concepts/ethereum-access-token\ndocs: https://docs.violet.co/for-developers/core-concepts\nnotes: >-\n  Violet has no traditional REST API with a securitySchemes block; its auth\n  model is an OAuth 2.0-compliant authorization flow that mints Ethereum\n  Access Tokens (EATs) plus on-chain verification against the VioletID\n  Registry. This profile is captured from the developer documentation\n  rather than derived from an OpenAPI spec.\nsummary:\n  types: [oauth2, onchain-registry]\n  token_format: EAT (EIP-712 signed message, OAuth 2.0 compliant, not JWT)\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: EthereumAccessToken\n    type: oauth2\n    flow: authorizationCode\n    token_format: EIP-712 signed message\n    description: >-\n      An Ethereum Access Token is a signed compliance assertion issued by the\n      Violet system (off-chain) and verified by the Violet Verifier\
  \ smart\n      contract (on-chain). It carries no direct PII; it only attests that a\n      wallet address has enrolled and satisfies the compliance requirements of\n      the integrating dApp. EATs are fully OAuth 2.0 compliant.\n    verifier_contract: \"0xe8F42626ba40be4478B4B13566E9B26faff33663\"  # AccessTokenVerifier, Ethereum Mainnet\n    source: https://docs.violet.co/for-developers/core-concepts/ethereum-access-token\n  - name: VioletIDRegistry\n    type: onchain-registry\n    description: >-\n      An on-chain registry mapping a wallet address to compliance statuses.\n      Any integrating dApp can query compliance status directly on-chain\n      without a round-trip to Violet; only Violet can modify entries. Used as\n      an alternative integration path to the EAT flow.\n    registry_contract: \"0xfFcDa323597A90af8F7A0eCBE4ef14e9b30e4a9e\"  # VioletID, Ethereum Mainnet\n    source: https://docs.violet.co/for-developers/core-concepts/violetid-registry\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/violet/refs/heads/main/authentication/violet-authentication.yml
summary_line: oauth2/onchain-registry · 2 schemes
tags:
- Company
- Compliance
- Identity
- DeFi
- Blockchain
- KYC
- AML
- Web3
- Decentralized Identity
- Sanctions Screening
- OAuth
---
