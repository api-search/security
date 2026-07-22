---
api_key_in: []
api_specs:
- filename: walrus-protocol-aggregator-openapi.json
  format: json
  label: Walrus Aggregator API
  slug: walrus-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walrus-protocol/refs/heads/main/openapi/walrus-protocol-aggregator-openapi.json
- filename: walrus-protocol-publisher-openapi.json
  format: json
  label: Walrus Publisher API
  slug: walrus-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walrus-protocol/refs/heads/main/openapi/walrus-protocol-publisher-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Walrus Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Walrus Protocol declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Walrus Protocol
provider_slug: walrus-protocol
scheme_count: 0
schemes: []
slug: walrus-protocol-authentication
source_filename: walrus-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/walrus-protocol-aggregator-openapi.json, openapi/walrus-protocol-publisher-openapi.json, https://docs.wal.app/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: none-by-default\nschemes: []\nnotes: >\n  Neither the Walrus Aggregator nor the Walrus Publisher OpenAPI declares any\n  securityScheme — the public HTTP daemons are unauthenticated. Reads (aggregator)\n  are open. Writes (publisher) cost WAL/SUI, so public publishers are best-effort\n  and rate/size limited; operators who run their own publisher typically gate it\n  behind their own layer (e.g. a JWT-authenticated upload relay) rather than a\n  Walrus-native auth scheme. On-chain operations (registering/certifying blobs,\n  paying with WAL) are authorized by Sui wallet signatures, not by an HTTP API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walrus-protocol/refs/heads/main/authentication/walrus-protocol-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Infrastructure
- Storage
- Decentralized Storage
- Blockchain
- Web3
- Data
- AI
- Sui
---
