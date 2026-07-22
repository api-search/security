---
api_key_in: []
auth_types: []
description: Authentication and authorization model for the Apptoken protocol suite. There are no API keys, no OAuth and no bearer tokens — the caller is authenticated by their EVM transaction signature, and delegated authority is granted through EIP-712 signed, time-bound approvals.
kind: authentication
layout: security
method: searched
name: Limit Break Authentication
name_suffix: Authentication
oauth_flows: []
overview: Limit Break declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Limit Break
provider_slug: limit-break
scheme_count: 6
schemes:
- description: The transaction sender (msg.sender) is the authenticated principal; authorization is enforced per-function by the contract.
  id: evm-transaction
  type: wallet-signature
- description: Off-chain typed-data signatures authorize orders that a third party submits on chain — Payment Processor listings and offers, TokenMaster advanced orders, and LBAMM permit swaps.
  docs:
  - https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/listings.md
  - https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/offers.md
  id: eip-712
  type: signature
- address: '0x000000fCE53B6fC312838A002362a9336F7ce39B'
  description: Time-bound, amount-bound token approvals with nonce management and a lockdown function, used as a safer alternative to ERC-20/721 approvalForAll.
  docs: https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/permits.md
  id: permitc
  type: delegated-approval
- description: Orders may require a second signature from a protocol- or exchange-controlled cosigner, allowing off-chain policy enforcement before a fill.
  docs: https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/cosigner-security.md
  id: cosigner
  type: co-signature
- description: Trusted Forwarder sits in front of the protocols to provide web2 app routing, attribution, and optional permissioning.
  docs: https://apptokens.com/docs/integration-guide/trusted-forwarder/overview.md
  factory: '0xFF0000B6c4352714cCe809000d0cd30A0E0c8DcE'
  id: trusted-forwarder
  type: meta-transaction
- description: Privileged operations are gated by contract roles, e.g. the FEE_MANAGER role that can adjust the Payment Processor protocol fee, and an infrastructure admin multisig for protocol-level bindings.
  id: role-based
  type: on-chain-roles
slug: limit-break-authentication
source_filename: limit-break-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apptokens.com/docs/ + skills/permitc-protocol/references/permitc-core.md\ndescription: Authentication and authorization model for the Apptoken protocol suite. There are no API keys, no OAuth\n  and no bearer tokens — the caller is authenticated by their EVM transaction signature, and delegated authority\n  is granted through EIP-712 signed, time-bound approvals.\nsurface: EVM smart contracts\nschemes:\n- id: evm-transaction\n  type: wallet-signature\n  description: The transaction sender (msg.sender) is the authenticated principal; authorization is enforced per-function\n    by the contract.\n- id: eip-712\n  type: signature\n  description: Off-chain typed-data signatures authorize orders that a third party submits on chain — Payment Processor\n    listings and offers, TokenMaster advanced orders, and LBAMM permit swaps.\n  docs:\n  - https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/listings.md\n\
  \  - https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/offers.md\n- id: permitc\n  type: delegated-approval\n  description: Time-bound, amount-bound token approvals with nonce management and a lockdown function, used as a\n    safer alternative to ERC-20/721 approvalForAll.\n  address: '0x000000fCE53B6fC312838A002362a9336F7ce39B'\n  docs: https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/permits.md\n- id: cosigner\n  type: co-signature\n  description: Orders may require a second signature from a protocol- or exchange-controlled cosigner, allowing\n    off-chain policy enforcement before a fill.\n  docs: https://apptokens.com/docs/integration-guide/payment-processor/v3.0/for-exchanges/cosigner-security.md\n- id: trusted-forwarder\n  type: meta-transaction\n  description: Trusted Forwarder sits in front of the protocols to provide web2 app routing, attribution, and optional\n    permissioning.\n  docs: https://apptokens.com/docs/integration-guide/trusted-forwarder/overview.md\n\
  \  factory: '0xFF0000B6c4352714cCe809000d0cd30A0E0c8DcE'\n- id: role-based\n  type: on-chain-roles\n  description: Privileged operations are gated by contract roles, e.g. the FEE_MANAGER role that can adjust the\n    Payment Processor protocol fee, and an infrastructure admin multisig for protocol-level bindings.\napi_keys: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: No apiKey, http, oauth2, openIdConnect or mutualTLS security schemes exist because Limit Break publishes\n  no HTTP API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limit-break/refs/heads/main/authentication/limit-break-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Gaming
- Blockchain
- Smart Contracts
- Ethereum
- EVM
- Tokens
- NFT
- DeFi
- Creator Economy
- Solidity
- Agent Skills
---
