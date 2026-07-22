---
api_key_in: []
api_specs:
- filename: nym-technologies-nym-api-openapi.json
  format: json
  label: Nym API
  slug: nym-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nym-technologies/refs/heads/main/openapi/nym-technologies-nym-api-openapi.json
- filename: nym-technologies-node-status-api-openapi.json
  format: json
  label: Node Status API
  slug: node-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nym-technologies/refs/heads/main/openapi/nym-technologies-node-status-api-openapi.json
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Nym Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nym Technologies secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nym Technologies
provider_slug: nym-technologies
scheme_count: 0
schemes: []
slug: nym-technologies-authentication
source_filename: nym-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nym-technologies-nym-api-openapi.json + https://nym.com/docs/apis/introduction\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  model: public-read\nnotes: >-\n  The Nym API (validator / nym-api) and Node Status API declare no OpenAPI\n  securitySchemes — they are public, unauthenticated read APIs for querying Nym\n  mixnet infrastructure. A handful of POST endpoints under /v1/ecash (blind-sign,\n  batch-redeem-ecash-tickets, verify-ecash-ticket) are protocol operations that\n  carry their own cryptographic integrity checks rather than API keys or OAuth:\n  requests are verified against ed25519 identity keys and rejected as\n  unauthorised (401) on failed integrity checks, or as stale/replayed (400).\n  There is no developer API key or OAuth token surface. Authentication for the\n  NymVPN product itself is handled out of band via anonymous zk-nym ecash\n  credentials, not via these query APIs.\nschemes:\
  \ []\nintegrity:\n  mechanism: ed25519-identity-key-signature\n  evidence:\n  - 401 responses read \"the submitted request was unauthorised or failed integrity check\"\n  - 400 responses read \"the submitted request is stale or replayed\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nym-technologies/refs/heads/main/authentication/nym-technologies-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Privacy
- VPN
- Mixnet
- Cryptography
- Decentralized
- Networking
- Web3
- Blockchain
- Anonymity
- Zero Knowledge
- Security
---
