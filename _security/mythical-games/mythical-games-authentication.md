---
api_key_in:
- grpc-metadata
auth_types:
- sdk-credential
description: ''
kind: authentication
layout: security
method: derived
name: Mythical Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mythical Games secures its APIs with sdk-credential across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mythical Games
provider_slug: mythical-games
scheme_count: 1
schemes:
- detail: SDK-managed credential presented as gRPC call metadata; title scoping via game_title_id / title_id request fields.
  in: metadata
  name: sdk-credential
  sources:
  - grpc/saga/
  type: apiKey
slug: mythical-games-authentication
source_filename: mythical-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: >-\n  grpc/saga/**/*.proto and the MythicalGames SDK repositories. No public OpenAPI\n  securitySchemes exist (this is a gRPC API); the model below is inferred from the\n  Protobuf contract and SDK usage.\nsummary:\n  types: [sdk-credential]\n  api_key_in: [grpc-metadata]\n  oauth2_flows: []\nnotes: >-\n  The Saga platform is a partner/B2B gRPC API accessed through first-party SDKs\n  (Java/C++/Python). There is no public OAuth/OpenID discovery surface. Requests are\n  scoped to a game title via game_title_id / title_id fields carried in the request\n  messages, and caller credentials are supplied via the SDK's environment\n  configuration (passed as gRPC call metadata). This artifact should be upgraded to\n  method:searched if Mythical publishes a partner authentication reference.\nschemes:\n- name: sdk-credential\n  type: apiKey\n  in: metadata\n  detail: >-\n    SDK-managed credential presented as gRPC call metadata; title\
  \ scoping via\n    game_title_id / title_id request fields.\n  sources: [grpc/saga/]\nscopes: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mythical-games/refs/heads/main/authentication/mythical-games-authentication.yml
summary_line: sdk-credential · 1 scheme
tags:
- Company
- Gaming
- Web3
- Blockchain
- Digital Assets
- NFT
- Marketplace
- gRPC
- SDK
- Game Platform
---
