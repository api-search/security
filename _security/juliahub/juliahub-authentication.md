---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Juliahub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
- tokenExchange
overview: Juliahub secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, refreshToken, and tokenExchange flow(s).
provider_name: Juliahub
provider_slug: juliahub
scheme_count: 3
schemes:
- issuer: https://auth.juliahub.com/dex
  name: OpenIDConnect
  openIdConnectUrl: https://juliahub.com/.well-known/openid-configuration
  sources:
  - well-known/juliahub-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.juliahub.com/dex/auth
    flow: authorizationCode
    tokenUrl: https://auth.juliahub.com/dex/token
  - deviceAuthorizationUrl: https://auth.juliahub.com/dex/device/code
    flow: deviceCode
    note: primary flow used by JuliaHub.jl and the jh CLI (urn:ietf:params:oauth:grant-type:device_code)
    tokenUrl: https://auth.juliahub.com/dex/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  name: OAuth2
  pkce:
  - S256
  - plain
  sources:
  - well-known/juliahub-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- bearerFormat: JWT
  name: BearerToken
  note: JWT id/access token minted by Dex, presented to JuliaHub platform APIs
  scheme: bearer
  sources:
  - https://github.com/JuliaComputing/jh
  type: http
slug: juliahub-authentication
source_filename: juliahub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://juliahub.com/.well-known/openid-configuration\ndocs: https://help.juliahub.com/julia-api/stable/guides/authentication/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken, tokenExchange]\n  bearer: true\n  notes: >-\n    JuliaHub authenticates via OpenID Connect / OAuth2 provided by a Dex\n    identity provider (issuer https://auth.juliahub.com/dex). The JuliaHub.jl\n    Julia client and the `jh` CLI both use the OAuth2 device-authorization\n    (device code) flow to obtain a JWT bearer token, which is then sent on\n    JuliaHub platform REST/GraphQL requests.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://juliahub.com/.well-known/openid-configuration\n  issuer: https://auth.juliahub.com/dex\n  sources: [well-known/juliahub-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n   \
  \ authorizationUrl: https://auth.juliahub.com/dex/auth\n    tokenUrl: https://auth.juliahub.com/dex/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.juliahub.com/dex/device/code\n    tokenUrl: https://auth.juliahub.com/dex/token\n    note: primary flow used by JuliaHub.jl and the jh CLI (urn:ietf:params:oauth:grant-type:device_code)\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  pkce: [S256, plain]\n  sources: [well-known/juliahub-openid-configuration.json]\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: JWT id/access token minted by Dex, presented to JuliaHub platform APIs\n  sources: [https://github.com/JuliaComputing/jh]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juliahub/refs/heads/main/authentication/juliahub-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Julia
- Scientific Computing
- Cloud Computing
- Modeling and Simulation
- High Performance Computing
- Data Science
- Developer Tools
- Package Registry
- Company
---
