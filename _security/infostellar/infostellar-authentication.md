---
api_key_in: []
auth_types:
- jwt-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Infostellar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infostellar secures its APIs with jwt-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infostellar
provider_slug: infostellar
scheme_count: 1
schemes:
- audience: https://api.stellarstation.com
  description: Authentication to the StellarStation gRPC API uses JWT bearer tokens signed with a service-account private key downloaded from the StellarStation Console. Credentials are registered as gRPC call credentials on the channel (e.g. ServiceAccountJwtAccessCredentials in Java, google-auth JWT OnDemandCredentials in Python). The token audience is https://api.stellarstation.com. Keys revoked in the Console stop working immediately.
  key_source: StellarStation Console (downloaded private key JSON)
  name: ServiceAccountJWT
  scheme: jwt
  sources:
  - grpc/infostellar-stellarstation.proto
  - README
  type: bearer
slug: infostellar-authentication
source_filename: infostellar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/infostellarinc/stellarstation-api#authentication\ndocs: https://github.com/infostellarinc/stellarstation-api#authentication\nsummary:\n  types: [jwt-bearer]\n  transport: grpc\n  token_kind: service-account-jwt\n  audience: https://api.stellarstation.com\nschemes:\n- name: ServiceAccountJWT\n  type: bearer\n  scheme: jwt\n  description: >-\n    Authentication to the StellarStation gRPC API uses JWT bearer tokens signed\n    with a service-account private key downloaded from the StellarStation\n    Console. Credentials are registered as gRPC call credentials on the channel\n    (e.g. ServiceAccountJwtAccessCredentials in Java, google-auth JWT\n    OnDemandCredentials in Python). The token audience is\n    https://api.stellarstation.com. Keys revoked in the Console stop working\n    immediately.\n  audience: https://api.stellarstation.com\n  key_source: StellarStation Console (downloaded private key JSON)\n\
  \  sources: [grpc/infostellar-stellarstation.proto, README]\nnotes: >-\n  gRPC over TLS on api.stellarstation.com:443. No API-key or OAuth2\n  authorization-code flow is documented; the only mechanism is service-account\n  JWT bearer credentials. There is no OAuth scope surface, so no scopes/\n  artifact applies.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infostellar/refs/heads/main/authentication/infostellar-authentication.yml
summary_line: jwt-bearer · 1 scheme
tags:
- Company
- Space
- Satellite
- Ground Station
- Aerospace
- Telemetry
- gRPC
- GSaaS
- Orbital
---
