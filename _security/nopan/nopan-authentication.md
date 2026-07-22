---
api_key_in: []
api_specs:
- filename: nopan-openapi-original.yml
  format: yaml
  label: Nopan API
  slug: nopan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nopan/refs/heads/main/openapi/nopan-openapi-original.yml
auth_types:
- oauth2
- mutualTLS
- http-bearer
- jws-signing
description: Nopan uses OAuth2 client_credentials machine-to-machine authentication layered over mutual TLS (mTLS), with every request additionally signed using JWS. The OpenAPI definition documents these in prose (tags and the /auth/token operation) rather than a formal components.securitySchemes block, so this profile is captured from the auth guide and the token operation.
kind: authentication
layout: security
method: searched
name: Nopan Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nopan secures its APIs with oauth2, mutualTLS, http-bearer, and jws-signing across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nopan
provider_slug: nopan
scheme_count: 4
schemes:
- client_id: organization account ID issued at onboarding
  default_scope: payments:read
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  scopes:
  - payments:read
  - payments:process
  source: openapi/nopan-openapi-original.yml#getAccessToken
  token_type: Bearer (JWT, ES256)
  token_url: https://api.nopan.io/auth/token
  type: oauth2
- description: Client certificate required on the TLS handshake for all requests (mTLS).
  name: MutualTLS
  type: mutualTLS
- bearer_format: JWT
  description: Access token from /auth/token presented as Authorization Bearer on protected resources.
  name: BearerToken
  scheme: bearer
  type: http
- description: Every request is signed with JWS (JSON Web Signature) and validated server-side.
  name: JWSRequestSigning
  type: message-signature
slug: nopan-authentication
source_filename: nopan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nopan.com/guides/authentication\ndocs: https://docs.nopan.com/guides/authentication\ndescription: >-\n  Nopan uses OAuth2 client_credentials machine-to-machine authentication layered\n  over mutual TLS (mTLS), with every request additionally signed using JWS. The\n  OpenAPI definition documents these in prose (tags and the /auth/token operation)\n  rather than a formal components.securitySchemes block, so this profile is captured\n  from the auth guide and the token operation.\nsummary:\n  types: [oauth2, mutualTLS, http-bearer, jws-signing]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.nopan.io/auth/token\n    grant_type: client_credentials\n    client_id: organization account ID issued at onboarding\n    token_type: Bearer (JWT, ES256)\n    default_scope: payments:read\n    scopes:\
  \ [payments:read, payments:process]\n    source: openapi/nopan-openapi-original.yml#getAccessToken\n  - name: MutualTLS\n    type: mutualTLS\n    description: Client certificate required on the TLS handshake for all requests (mTLS).\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: Access token from /auth/token presented as Authorization Bearer on protected resources.\n  - name: JWSRequestSigning\n    type: message-signature\n    description: Every request is signed with JWS (JSON Web Signature) and validated server-side.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nopan/refs/heads/main/authentication/nopan-authentication.yml
summary_line: oauth2/mutualTLS/http-bearer/jws-signing · 4 schemes
tags:
- Payments
- Payment Service Provider
- Account to Account
- Wallet Payments
- Open Banking
- PSD2
- Fintech
- Europe
- Tokenization
- Recurring Payments
---
