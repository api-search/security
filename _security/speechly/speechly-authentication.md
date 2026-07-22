---
api_key_in: []
auth_types:
- oauth2-like
- bearer
description: ''
kind: authentication
layout: security
method: derived
name: Speechly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speechly secures its APIs with oauth2-like and bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Speechly
provider_slug: speechly
scheme_count: 1
schemes:
- description: 'IdentityAPI.Login(LoginRequest{device_id, scope: application|project}) returns a LoginResponse access token used as the gRPC Authorization bearer credential for SLU, WLU, Batch, Config, Analytics and Moderation services.'
  name: identityLogin
  scheme: bearer
  sources:
  - grpc/speechly/identity/v2/identity_api.proto
  - grpc/speechly/identity/v1/identity.proto
  type: token-exchange
slug: speechly-authentication
source_filename: speechly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: grpc/speechly/identity/v2/identity_api.proto\nnote: >-\n  Speechly used a two-step gRPC auth model: exchange an application/project\n  identifier plus device id for a short-lived bearer access token via the\n  Identity API, then present the token as gRPC metadata on subsequent calls.\n  Derived from the archived protobuf definitions; the hosted API is discontinued.\nsummary:\n  types: [oauth2-like, bearer]\n  token_endpoint: speechly.identity.v2.IdentityAPI/Login\nschemes:\n  - name: identityLogin\n    type: token-exchange\n    scheme: bearer\n    description: >-\n      IdentityAPI.Login(LoginRequest{device_id, scope: application|project})\n      returns a LoginResponse access token used as the gRPC Authorization\n      bearer credential for SLU, WLU, Batch, Config, Analytics and Moderation\n      services.\n    sources:\n      - grpc/speechly/identity/v2/identity_api.proto\n      - grpc/speechly/identity/v1/identity.proto\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speechly/refs/heads/main/authentication/speechly-authentication.yml
summary_line: oauth2-like/bearer · 1 scheme
tags:
- Company
- Speech Recognition
- Voice
- Spoken Language Understanding
- Speech-to-Text
- Content Moderation
- Machine Learning
- gRPC
- Artificial Intelligence
---
