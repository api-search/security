---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kixeye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kixeye secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kixeye
provider_slug: kixeye
scheme_count: 1
schemes:
- claims_supported:
  - iss
  - aud
  - nbf
  - iat
  - exp
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.kixeye.com
  jwks_uri: https://api.kixeye.com/.well-known/jwks
  name: kixeye-oidc
  openIdConnectUrl: https://api.kixeye.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/kixeye-openid-configuration.json
  - well-known/kixeye-jwks.json
  type: openIdConnect
slug: kixeye-authentication
source_filename: kixeye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.kixeye.com/.well-known/openid-configuration\nnotes: 'KIXEYE publishes no public API and no developer authentication documentation. The only observable\n  authentication surface is the OpenID Connect discovery document served by the private game-services\n  backend at api.kixeye.com, captured verbatim in well-known/. This profile is derived from that document\n  only — it describes how KIXEYE signs and verifies its own player tokens, not a partner-facing auth\n  model. No authorization_endpoint or token_endpoint is advertised, so the discovery document is a\n  verification-only (JWKS publication) profile.'\nsummary:\n  types:\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: kixeye-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://api.kixeye.com/.well-known/openid-configuration\n  issuer: https://api.kixeye.com\n  jwks_uri: https://api.kixeye.com/.well-known/jwks\n  response_types_supported:\n\
  \  - code\n  id_token_signing_alg_values_supported:\n  - RS256\n  claims_supported:\n  - iss\n  - aud\n  - nbf\n  - iat\n  - exp\n  sources:\n  - well-known/kixeye-openid-configuration.json\n  - well-known/kixeye-jwks.json\njwks:\n  keys: 1\n  kty: RSA\n  alg: RS256\n  use: sig\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kixeye/refs/heads/main/authentication/kixeye-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Gaming
- Video Games
- Game Development
- Mobile Games
- Strategy Games
- Free To Play
- Live Service
---
