---
api_key_in: []
api_specs:
- filename: bigchaindb-http-openapi.yml
  format: yaml
  label: BigchainDB HTTP API
  slug: bigchaindb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchaindb/refs/heads/main/openapi/bigchaindb-http-openapi.yml
auth_types:
- none
- payload-signature
description: ''
kind: authentication
layout: security
method: searched
name: Bigchaindb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bigchaindb secures its APIs with none and payload-signature across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bigchaindb
provider_slug: bigchaindb
scheme_count: 0
schemes: []
slug: bigchaindb-authentication
source_filename: bigchaindb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  BigchainDB Server HTTP API reference and transaction-model documentation.\n  Derived-then-confirmed: the OpenAPI transcription declares no HTTP\n  securitySchemes because the BigchainDB HTTP API has no transport-layer auth by\n  default — authorization is enforced cryptographically at the payload level.\ndocs: https://docs.bigchaindb.com/projects/server/en/latest/http-client-server-api.html\nsummary:\n  types: [none, payload-signature]\n  api_key_in: []\n  oauth2_flows: []\nmodel:\n  transport_auth: none-by-default\n  payload_auth: crypto-conditions (Ed25519 signatures)\n  notes: >-\n    The core BigchainDB HTTP API accepts unauthenticated reads and writes; a write\n    is only valid if the transaction is correctly signed with the owners' Ed25519\n    keys via crypto-conditions, and outputs can only be spent by fulfilling their\n    conditions. Hosted networks may add app_id / app_key headers at the gateway\n    (deployment-specific),\
  \ but that is not part of the core API contract.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigchaindb/refs/heads/main/authentication/bigchaindb-authentication.yml
summary_line: none/payload-signature · 0 schemes
tags:
- Company
- Crypto
- Blockchain
- Database
- Decentralization
- Distributed Ledger
- Assets
- Immutability
---
