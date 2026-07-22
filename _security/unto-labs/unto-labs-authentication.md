---
api_key_in: []
auth_types:
- signature-based
description: ''
kind: authentication
layout: security
method: searched
name: Unto Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unto Labs secures its APIs with signature-based across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unto Labs
provider_slug: unto-labs
scheme_count: 0
schemes: []
slug: unto-labs-authentication
source_filename: unto-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thru.org/docs (DevKit setup, wallet integration, gRPC API reference)\nsummary:\n  types: [signature-based]\n  api_key_in: []\n  oauth2_flows: []\nmodel:\n  reads: The public Alphanet gRPC endpoint (https://rpc.alphanet.thru.org) is\n    documented without API keys or tokens — QueryService and StreamingService\n    reads are open.\n  writes: State-changing operations (CommandService SendTransaction /\n    BatchSendTransactions / SendAndTrackTxn) are authorized by transaction\n    signatures from user-held keypairs, not by API credentials.\ncredentials:\n  - kind: local-keypair\n    description: Keypairs are generated and stored locally by the CLI (thru keys\n      generate <name>, stored as plaintext hex in ~/.thru/cli/config.yaml).\n      Addresses and signatures use thrufmt encoding (ta.../ts...).\n  - kind: embedded-wallet\n    description: Browser apps integrate the hosted Thru wallet via @thru/wallet\n      (approval\
  \ and signing flows documented under wallet integration).\n    docs: https://thru.org/docs/wallet/overview/\n  - kind: passkey\n    description: Cross-platform passkey helpers via @thru/passkey for\n      authenticating Thru applications.\nexternal_signers:\n  docs: https://thru.org/docs (C SDK reference, External Signers)\nnotes:\n  - No OAuth2, OpenID Connect, API-key, or mutual-TLS scheme is published; scopes/ is not applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unto-labs/refs/heads/main/authentication/unto-labs-authentication.yml
summary_line: signature-based · 0 schemes
tags:
- Company
- Crypto
- Blockchain
- Layer 1
- RISC-V
- Virtual Machines
- gRPC
- Web3
- Infrastructure
---
