---
api_key_in: []
auth_types:
- substrate-keypair-signature
description: ''
kind: authentication
layout: security
method: searched
name: Bittensor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bittensor secures its APIs with substrate-keypair-signature across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bittensor
provider_slug: bittensor
scheme_count: 0
schemes: []
slug: bittensor-authentication
source_filename: bittensor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.bittensor.com/docs/concepts/wallets\nsummary:\n  model: wallet-key-signing\n  types:\n  - substrate-keypair-signature\n  no_oauth: true\n  no_api_keys: true\n  note: Bittensor has no hosted REST API and therefore no API keys or OAuth. Every state-changing operation\n    is a Substrate extrinsic signed by a wallet keypair; there is no bearer token or account SID.\nkeys:\n- name: coldkey\n  role: Custodial root key; authorizes funds and high-value operations; kept offline where possible.\n- name: hotkey\n  role: Operational key registered on subnets to mine/validate and to sign inter-neuron HTTP requests.\nsignature_schemes:\n- sr25519\n- ed25519\nsigning_methods:\n- method: sdk/cli\n  docs: https://www.bittensor.com/docs/quickstart\n- method: browser-extension\n  detail: Talisman / Polkadot.js — key never touches the CLI host.\n  docs: https://www.bittensor.com/docs/guides/extension-signing\n- method: ledger\n  detail:\
  \ Polkadot generic app on Ledger hardware wallet.\n  docs: https://www.bittensor.com/docs/guides/ledger\n- method: proxy\n  detail: Scoped, revocable delegate keys sign day-to-day calls for an offline coldkey.\n  docs: https://www.bittensor.com/docs/guides/proxies\n- method: multisig\n  detail: M-of-N control of a coldkey.\n  docs: https://www.bittensor.com/docs/guides/multisig\nrequest_auth:\n  scheme: btauth/1\n  description: Hotkey-signed HTTP between validators and miners (signed-requests wire format).\n  docs: https://www.bittensor.com/docs/guides/signed-requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bittensor/refs/heads/main/authentication/bittensor-authentication.yml
summary_line: substrate-keypair-signature · 0 schemes
tags:
- Company
- Ai
- Blockchain
- Decentralized AI
- Machine Learning
- Cryptocurrency
- Web3
- SDK
- CLI
- DePIN
---
