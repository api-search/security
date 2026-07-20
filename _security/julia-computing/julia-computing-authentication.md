---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Julia Computing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
- tokenExchange
overview: Julia Computing secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, refreshToken, and tokenExchange flow(s).
provider_name: Julia Computing
provider_slug: julia-computing
scheme_count: 1
schemes:
- authorization_endpoint: https://auth.juliahub.com/dex/auth
  code_challenge_methods_supported:
  - S256
  - plain
  device_authorization_endpoint: https://auth.juliahub.com/dex/device/code
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://auth.juliahub.com/dex/token/introspect
  issuer: https://auth.juliahub.com/dex
  jwks_uri: https://auth.juliahub.com/dex/keys
  name: OpenIDConnect
  openIdConnectUrl: https://juliahub.com/.well-known/openid-configuration
  sources:
  - well-known/julia-computing-openid-configuration.json
  token_endpoint: https://auth.juliahub.com/dex/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://auth.juliahub.com/dex/userinfo
slug: julia-computing-authentication
source_filename: julia-computing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://juliahub.com/.well-known/openid-configuration\ndocs: https://help.juliahub.com/juliahub-jl/stable/getting-started/\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, deviceCode, refreshToken, tokenExchange]\n  pkce: true\n  notes: JuliaHub authenticates users and API clients via an OpenID Connect provider built on Dex. The first-party JuliaHub.jl client authenticates through this flow (PkgAuthentication.jl handles package-server auth).\nschemes:\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://juliahub.com/.well-known/openid-configuration\n    issuer: https://auth.juliahub.com/dex\n    authorization_endpoint: https://auth.juliahub.com/dex/auth\n    token_endpoint: https://auth.juliahub.com/dex/token\n    userinfo_endpoint: https://auth.juliahub.com/dex/userinfo\n    device_authorization_endpoint: https://auth.juliahub.com/dex/device/code\n    introspection_endpoint:\
  \ https://auth.juliahub.com/dex/token/introspect\n    jwks_uri: https://auth.juliahub.com/dex/keys\n    grant_types_supported: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:device_code\", \"urn:ietf:params:oauth:grant-type:token-exchange\"]\n    code_challenge_methods_supported: [S256, plain]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    sources: [well-known/julia-computing-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julia-computing/refs/heads/main/authentication/julia-computing-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Julia
- Scientific Computing
- Modeling and Simulation
- High Performance Computing
- Cloud Computing
- Data Science
- Programming Language
- Package Registry
- Machine Learning
- Pharma
---
