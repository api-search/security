---
api_key_in: []
auth_types: []
description: 'Authentication profile assembled from Lootex''s open-source core and Forge developer documentation. Two distinct surfaces existed: the marketplace backend used Web3 wallet signature authentication issuing JWTs, while the Forge minting/developer API used per-application API keys issued after registration.'
kind: authentication
layout: security
method: searched
name: Lootex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lootex declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Lootex
provider_slug: lootex
scheme_count: 3
schemes:
- description: Users authenticate by signing a challenge with their Web3 wallet; the backend verifies the signature and issues a JWT for subsequent requests.
  in: null
  name: Wallet signature (SIWE-style)
  source: https://github.com/lootex-io/lootex-core
  type: web3-signature
- bearer_format: JWT
  description: Session JWT returned after wallet authentication, presented as a Bearer token on marketplace API calls.
  in: header
  location: Authorization
  name: JWT bearer
  scheme: bearer
  source: https://github.com/lootex-io/lootex-core
  type: http
- description: The Forge developer/minting API required each client to register their application and request an API key. The Forge developer portal (docs.forge.lootex.dev) is no longer resolving.
  in: header
  location: null
  name: Forge API key
  source: https://github.com/Howard86/lootex-api
  type: apiKey
slug: lootex-authentication
source_filename: lootex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/lootex-io/lootex-core\nname: Lootex Authentication\ndescription: >-\n  Authentication profile assembled from Lootex's open-source core and Forge\n  developer documentation. Two distinct surfaces existed: the marketplace\n  backend used Web3 wallet signature authentication issuing JWTs, while the\n  Forge minting/developer API used per-application API keys issued after\n  registration.\nschemes:\n- type: web3-signature\n  name: Wallet signature (SIWE-style)\n  description: >-\n    Users authenticate by signing a challenge with their Web3 wallet; the\n    backend verifies the signature and issues a JWT for subsequent requests.\n  in: null\n  source: https://github.com/lootex-io/lootex-core\n- type: http\n  scheme: bearer\n  bearer_format: JWT\n  name: JWT bearer\n  description: >-\n    Session JWT returned after wallet authentication, presented as a Bearer\n    token on marketplace API calls.\n  in: header\n\
  \  location: Authorization\n  source: https://github.com/lootex-io/lootex-core\n- type: apiKey\n  name: Forge API key\n  description: >-\n    The Forge developer/minting API required each client to register their\n    application and request an API key. The Forge developer portal\n    (docs.forge.lootex.dev) is no longer resolving.\n  in: header\n  location: null\n  source: https://github.com/Howard86/lootex-api\nnotes: >-\n  No OpenAPI/Swagger definition is published, so securitySchemes could not be\n  derived from a spec. This profile is grounded in the public repositories and\n  developer documentation only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lootex/refs/heads/main/authentication/lootex-authentication.yml
summary_line: 3 schemes
tags:
- Company
- NFT
- Marketplace
- Web3
- Blockchain
- Digital Assets
- Minting
---
