---
api_key_in: []
auth_types:
- challenge-response
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Harmonic Gg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harmonic GG secures its APIs with challenge-response and bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Harmonic GG
provider_slug: harmonic-gg
scheme_count: 2
schemes:
- description: Clients authenticate by proving control of a Solana keypair. The client calls GenerateAuthChallenge with its role and 32-byte pubkey, signs the returned challenge (the client signs "{pubkey}-{challenge}"), then exchanges the signed challenge via GenerateAuthTokens for an access token and a longer-lived refresh token. RefreshAccessToken mints a fresh access token before expiry.
  name: KeypairChallengeResponse
  operations:
  - GenerateAuthChallenge
  - GenerateAuthTokens
  - RefreshAccessToken
  roles:
    note: Harmonic uses Role.SEARCHER = 3, which differs from jito-protos where SEARCHER = 1. Reusing jito-protos clients requires authenticating with the ShredstreamSubscriber role (= 3).
    values:
    - name: ROLE_UNSPECIFIED
      value: 0
    - name: SEARCHER
      value: 3
  service: auth.AuthService
  transport: grpc
  type: challenge-response
- description: Each request carries the access token as a gRPC Bearer credential. Reference client interceptors add the token automatically, refresh it ~5 minutes before expiry, and re-authenticate when the refresh token expires.
  location: metadata
  name: BearerToken
  transport: grpc
  type: bearer
slug: harmonic-gg-authentication
source_filename: harmonic-gg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.harmonic.gg/searchers/harmonic-bundles\ndocs: https://docs.harmonic.gg/searchers/harmonic-bundles\ngrpc_source:\n- grpc/harmonic-gg-searcher-auth.proto\n- grpc/harmonic-gg-validator-auth.proto\nsummary:\n  types:\n  - challenge-response\n  - bearer\n  model: Solana-keypair challenge-response issuing short-lived Bearer access + refresh tokens over gRPC metadata; there is no API key or OAuth surface.\n  allowlist_required: true\nschemes:\n- name: KeypairChallengeResponse\n  type: challenge-response\n  transport: grpc\n  service: auth.AuthService\n  description: >-\n    Clients authenticate by proving control of a Solana keypair. The client calls\n    GenerateAuthChallenge with its role and 32-byte pubkey, signs the returned\n    challenge (the client signs \"{pubkey}-{challenge}\"), then exchanges the signed\n    challenge via GenerateAuthTokens for an access token and a longer-lived refresh\n    token. RefreshAccessToken\
  \ mints a fresh access token before expiry.\n  operations:\n  - GenerateAuthChallenge\n  - GenerateAuthTokens\n  - RefreshAccessToken\n  roles:\n    note: Harmonic uses Role.SEARCHER = 3, which differs from jito-protos where SEARCHER = 1. Reusing jito-protos clients requires authenticating with the ShredstreamSubscriber role (= 3).\n    values:\n    - {name: ROLE_UNSPECIFIED, value: 0}\n    - {name: SEARCHER, value: 3}\n- name: BearerToken\n  type: bearer\n  transport: grpc\n  location: metadata\n  description: >-\n    Each request carries the access token as a gRPC Bearer credential. Reference\n    client interceptors add the token automatically, refresh it ~5 minutes before\n    expiry, and re-authenticate when the refresh token expires.\nauthorization:\n  allowlist:\n    description: Beyond token auth, the searcher pubkey (or validator identity) must be whitelisted by the Harmonic team before requests are accepted; a non-whitelisted key is rejected with permission denied.\n    searcher_intake:\
  \ https://form.typeform.com/to/aUd0FiwD\n    validator_intake: https://form.typeform.com/to/UlJMfbPH\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic-gg/refs/heads/main/authentication/harmonic-gg-authentication.yml
summary_line: challenge-response/bearer · 2 schemes
tags:
- Company
- Blockchain
- Solana
- Block Building
- MEV
- Validator
- Searcher
- Infrastructure
- gRPC
- DeFi
---
