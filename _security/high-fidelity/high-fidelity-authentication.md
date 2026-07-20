---
api_key_in: []
auth_types:
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: High Fidelity Authentication
name_suffix: Authentication
oauth_flows: []
overview: High Fidelity secures its APIs with jwt across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: High Fidelity
provider_slug: high-fidelity
scheme_count: 1
schemes:
- description: Clients connect to the High Fidelity Spatial Audio API server by supplying a JSON Web Token (JWT) to HiFiCommunicator.connectToHiFiAudioAPIServer(). The JWT is signed with the developer's App Secret and encodes the App ID and the target Space (audio environment). Credentials (App ID, App Secret, Space) are issued from a free High Fidelity Developer Account.
  name: SpatialAudioJWT
  required_credentials:
  - App ID
  - App Secret
  - Space (name/id)
  scheme: bearer
  signup: https://account.highfidelity.com
  sources:
  - github.com/highfidelity/hifi-spatial-audio-js (README)
  type: jwt
slug: high-fidelity-authentication
source_filename: high-fidelity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/highfidelity/hifi-spatial-audio-js#readme\ndocs: https://www.highfidelity.com/api/guides/misc/getAJWT\nsummary:\n  types: [jwt]\n  transport: connection-token\n  credential_source: High Fidelity Developer Account (account.highfidelity.com)\nschemes:\n  - name: SpatialAudioJWT\n    type: jwt\n    scheme: bearer\n    description: >-\n      Clients connect to the High Fidelity Spatial Audio API server by supplying\n      a JSON Web Token (JWT) to HiFiCommunicator.connectToHiFiAudioAPIServer().\n      The JWT is signed with the developer's App Secret and encodes the App ID\n      and the target Space (audio environment). Credentials (App ID, App Secret,\n      Space) are issued from a free High Fidelity Developer Account.\n    required_credentials:\n      - App ID\n      - App Secret\n      - Space (name/id)\n    signup: https://account.highfidelity.com\n    sources:\n      - github.com/highfidelity/hifi-spatial-audio-js\
  \ (README)\nnotes: >-\n  Derived from the published SDK README and the getAJWT guide rather than an\n  OpenAPI securityScheme (no OpenAPI is published). The hosted service that\n  validated these JWTs has since been discontinued; the auth model is recorded\n  as documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-fidelity/refs/heads/main/authentication/high-fidelity-authentication.yml
summary_line: jwt · 1 scheme
tags:
- Company
- Consumer
- Spatial Audio
- Audio
- Voice
- WebRTC
- SDK
- Real-Time Communication
- Gaming
---
