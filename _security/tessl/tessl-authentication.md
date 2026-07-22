---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tessl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tessl secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tessl
provider_slug: tessl
scheme_count: 2
schemes:
- authorization_endpoint: https://auth.tessl.io/oauth2/authorize
  device_authorization_endpoint: https://auth.tessl.io/oauth2/device_authorization
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://auth.tessl.io/oauth2/introspection
  jwks_uri: https://auth.tessl.io/oauth2/jwks
  name: OAuth2 / OpenID Connect
  openIdConnectUrl: https://auth.tessl.io/.well-known/openid-configuration
  sources:
  - auth.tessl.io/.well-known/openid-configuration
  token_endpoint: https://auth.tessl.io/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://auth.tessl.io/oauth2/userinfo
- description: 'Workspace-scoped API key minted with `tessl api-key create` (roles: member, publisher, manager, owner; optional expiry). Used for CI / non-interactive contexts in place of the interactive device-code login.'
  env: TESSL_TOKEN
  in: header
  name: Tessl API key
  sources:
  - docs.tessl.io/reference/cli-commands.md
  type: apiKey
slug: tessl-authentication
source_filename: tessl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.tessl.io/.well-known/openid-configuration\ndocs: https://docs.tessl.io/introduction-to-tessl/set-up-tessl/installation.md\n# Tessl has no OpenAPI, so this profile is captured from the live OIDC discovery\n# document and the CLI/docs auth flow rather than derived from a spec.\nsummary:\n  types: [oauth2, openIdConnect]\n  primary_flow: device_code\n  identity_providers: [GitHub, Google]\n  api_key: workspace-scoped (tessl api-key create; TESSL_TOKEN env for CI)\nissuer: https://auth.tessl.io\nschemes:\n  - name: OAuth2 / OpenID Connect\n    type: openIdConnect\n    openIdConnectUrl: https://auth.tessl.io/.well-known/openid-configuration\n    authorization_endpoint: https://auth.tessl.io/oauth2/authorize\n    token_endpoint: https://auth.tessl.io/oauth2/token\n    device_authorization_endpoint: https://auth.tessl.io/oauth2/device_authorization\n    userinfo_endpoint: https://auth.tessl.io/oauth2/userinfo\n    introspection_endpoint:\
  \ https://auth.tessl.io/oauth2/introspection\n    jwks_uri: https://auth.tessl.io/oauth2/jwks\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n    sources: [auth.tessl.io/.well-known/openid-configuration]\n  - name: Tessl API key\n    type: apiKey\n    in: header\n    env: TESSL_TOKEN\n    description: >-\n      Workspace-scoped API key minted with `tessl api-key create` (roles: member,\n      publisher, manager, owner; optional expiry). Used for CI / non-interactive\n      contexts in place of the interactive device-code login.\n    sources: [docs.tessl.io/reference/cli-commands.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessl/refs/heads/main/authentication/tessl-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Ai
- Agents
- Agentic Development
- Developer Tools
- Agent Skills
- MCP
- CLI
- Registry
- Code Review
---
