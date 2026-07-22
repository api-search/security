---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Anoma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anoma secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anoma
provider_slug: anoma
scheme_count: 1
schemes:
- name: discovery-keypair
  operation: IndexerClient.addKeys
  scheme: keypair-registration
  sources:
  - docs.anoma.net/api-clients
  - docs.anoma.net/key-management
  type: cryptographic
slug: anoma-authentication
source_filename: anoma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.anoma.net/api-clients\ndocs: https://docs.anoma.net/key-management\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Anoma's App SDK API clients do not use traditional API-key or OAuth\n    authentication. Clients are constructed with a service URL. On-chain identity\n    and access are handled through cryptographic key management: the IndexerClient\n    registers discovery keypairs (addKeys) and transactions are proven and settled\n    via the Anoma Resource Machine rather than authenticated with bearer tokens.\nschemes:\n- name: discovery-keypair\n  type: cryptographic\n  scheme: keypair-registration\n  operation: IndexerClient.addKeys\n  sources: [docs.anoma.net/api-clients, docs.anoma.net/key-management]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anoma/refs/heads/main/authentication/anoma-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Infrastructure
- Blockchain
- Intents
- Privacy
- SDK
- Web3
- Decentralized
---
