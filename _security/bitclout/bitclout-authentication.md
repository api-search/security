---
api_key_in: []
auth_types:
- derived-keys
- transaction-signing
description: ''
kind: authentication
layout: security
method: searched
name: Bitclout Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitClout secures its APIs with derived-keys and transaction-signing across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BitClout
provider_slug: bitclout
scheme_count: 3
schemes:
- contexts:
  - iframe
  - window
  description: Browser-embedded identity provider. The iframe context handles background requests (transaction signing, message decryption); the window context handles interactive flows (log in, sign up, account management). Communicates via window.postMessage message events.
  docs: https://docs.deso.org/deso-identity/identity
  name: DeSo Identity Service
  type: identity-service
- description: Scoped, revocable keys authorized by a master key with transaction spending limits (per-transaction-type and global $DESO caps). Used for server-side and delegated signing without exposing the master seed.
  docs: https://docs.deso.org/deso-backend/construct-transactions/derived-keys-transaction-api
  name: Derived Keys
  type: derived-key
- description: Fine-grained authorization attached to derived keys constraining which transaction types (and how much $DESO) a key may spend.
  docs: https://docs.deso.org/deso-backend/api/transaction-spending-limits-endpoints
  name: Transaction Spending Limits
  type: authorization-policy
slug: bitclout-authentication
source_filename: bitclout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.deso.org/deso-identity/identity/concepts\ndocs: https://docs.deso.org/deso-identity/identity\nsummary:\n  model: blockchain-keypair\n  types: [derived-keys, transaction-signing]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    DeSo does not use API keys, OAuth, or bearer tokens for its backend API.\n    Read/data endpoints are public and permissionless. Write operations are\n    two-step: a node constructs an unsigned transaction, the client signs it with\n    a user's (or derived) key via the DeSo Identity Service, and submits the\n    signed transaction back to the node.\nschemes:\n- name: DeSo Identity Service\n  type: identity-service\n  contexts: [iframe, window]\n  description: >-\n    Browser-embedded identity provider. The iframe context handles background\n    requests (transaction signing, message decryption); the window context\n    handles interactive flows (log in, sign up, account management).\
  \ Communicates\n    via window.postMessage message events.\n  docs: https://docs.deso.org/deso-identity/identity\n- name: Derived Keys\n  type: derived-key\n  description: >-\n    Scoped, revocable keys authorized by a master key with transaction spending\n    limits (per-transaction-type and global $DESO caps). Used for server-side and\n    delegated signing without exposing the master seed.\n  docs: https://docs.deso.org/deso-backend/construct-transactions/derived-keys-transaction-api\n- name: Transaction Spending Limits\n  type: authorization-policy\n  description: >-\n    Fine-grained authorization attached to derived keys constraining which\n    transaction types (and how much $DESO) a key may spend.\n  docs: https://docs.deso.org/deso-backend/api/transaction-spending-limits-endpoints\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitclout/refs/heads/main/authentication/bitclout-authentication.yml
summary_line: derived-keys/transaction-signing · 3 schemes
tags:
- Company
- Blockchain
- Web3
- Decentralized Social
- Social
- Cryptocurrency
- NFT
- Creator Economy
- Identity
- Developer Tools
---
