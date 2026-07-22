---
api_key_in: []
api_specs:
- filename: proof-of-play-vrf-openapi.json
  format: json
  label: Proof of Play vRNG API
  slug: proof-of-play-vrng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proof-of-play/refs/heads/main/openapi/proof-of-play-vrf-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Proof Of Play Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proof of Play secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Proof of Play
provider_slug: proof-of-play
scheme_count: 1
schemes:
- applied_to:
  - PublicController_process
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/proof-of-play-vrf-openapi.json
  type: http
slug: proof-of-play-authentication
source_filename: proof-of-play-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/proof-of-play-vrf-openapi.json\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  The Proof of Play vRNG OpenAPI declares a global security requirement of\n  `bearerAuth` (HTTP bearer token) on the single public operation, but the spec\n  does not define the scheme under components.securitySchemes, so the bearer\n  format is not published. Calls to GET /v1/vrf/{chainId}/{txHash} carry an\n  Authorization: Bearer <token> header.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  applied_to: [PublicController_process]\n  sources: [openapi/proof-of-play-vrf-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proof-of-play/refs/heads/main/authentication/proof-of-play-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Gaming
- Blockchain
- Web3
- Randomness
- Onchain Infrastructure
- NFT
- Developer Services
---
