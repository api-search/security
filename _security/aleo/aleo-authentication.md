---
api_key_in: []
api_specs:
- filename: aleo-blocks-api-openapi.yml
  format: yaml
  label: Aleo Blocks API
  slug: aleo-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/openapi/aleo-blocks-api-openapi.yml
- filename: aleo-chain-api-openapi.yml
  format: yaml
  label: Aleo Chain API
  slug: aleo-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/openapi/aleo-chain-api-openapi.yml
- filename: aleo-network-api-openapi.yml
  format: yaml
  label: Aleo Network API
  slug: aleo-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/openapi/aleo-network-api-openapi.yml
- filename: aleo-programs-api-openapi.yml
  format: yaml
  label: Aleo Programs API
  slug: aleo-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/openapi/aleo-programs-api-openapi.yml
- filename: aleo-transactions-api-openapi.yml
  format: yaml
  label: Aleo Transactions API
  slug: aleo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/openapi/aleo-transactions-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Aleo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aleo secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aleo
provider_slug: aleo
scheme_count: 0
schemes: []
slug: aleo-authentication
source_filename: aleo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.aleo.org/ + live probe of api.explorer.provable.com\nsummary:\n  types: [none]\n  note: >-\n    The public Aleo node REST API (api.explorer.provable.com) is unauthenticated.\n    Read endpoints (chain state, blocks, transactions, programs, mappings,\n    committee) require no API key, token, or credential. Write access is not\n    granted via HTTP auth — the POST /transaction/broadcast endpoint accepts a\n    transaction that is already cryptographically signed with the sender's Aleo\n    private key (the on-chain authorization model), so authorization is enforced\n    by zk-proof and signature validation at the protocol layer, not by API\n    credentials. Aleo accounts are keypairs (private key / view key / address)\n    generated with the Provable SDK or the Leo CLI account commands.\nschemes: []\naccount_model:\n  identity: Aleo account keypair (APrivateKey / AViewKey / aleo1... address)\n  signing: Transactions\
  \ are authorized and signed with the account private key via snarkVM / the Provable SDK before broadcast.\n  docs: https://docs.aleo.org/build/leo/documentation/cli/cli_account/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/authentication/aleo-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Blockchain
- Zero-Knowledge
- Cryptography
- Privacy
- Web3
- Developer Tools
- Cryptocurrency
- Smart Contracts
---
