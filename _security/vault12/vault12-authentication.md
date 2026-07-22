---
api_key_in: []
auth_types:
- oauth2
- session-handshake
description: ''
kind: authentication
layout: security
method: searched
name: Vault12 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- refresh_token
overview: Vault12 secures its APIs with oauth2 and session-handshake across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and refresh_token flow(s).
provider_name: Vault12
provider_slug: vault12
scheme_count: 2
schemes:
- authorizationUrl: https://vault12.com/core/users/oauth2/authorize
  issuer: https://vault12.com
  jwksUrl: https://vault12.com/core/users/oauth2/jwks
  name: Vault12OAuth2
  registrationUrl: https://vault12.com/core/users/oauth2/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/vault12-oauth-authorization-server.json
  tokenUrl: https://vault12.com/core/users/oauth2/token
  type: oauth2
  userinfoUrl: https://vault12.com/core/users/oauth2/user_info
- description: 'Anonymous per-session NaCl key establishment on Zax relay nodes: POST /start_session with a random token returns a proof-of-work challenge; POST /verify_session answers it and yields temporary session keys; subsequent POST /command requests are encrypted with the session keys. No long-term credentials or API keys.'
  name: ZaxSessionHandshake
  sources:
  - https://github.com/vault12/zax
  type: custom
slug: vault12-authentication
source_filename: vault12-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://vault12.com/.well-known/oauth-authorization-server\nnotes: >-\n  No OpenAPI is published, so this profile is captured from the RFC 8414\n  authorization-server metadata Vault12 publishes on vault12.com plus the\n  open-source Zax relay protocol (https://github.com/vault12/zax). The Zax\n  relay uses no account credentials at all: clients establish per-session\n  NaCl keys via a /start_session proof-of-work handshake and /verify_session,\n  then send session-key-encrypted commands to /command.\nsummary:\n  types: [oauth2, session-handshake]\n  oauth2_flows: [authorizationCode, implicit, password, refresh_token]\n  pkce: [plain, S256]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\nschemes:\n  - name: Vault12OAuth2\n    type: oauth2\n    issuer: https://vault12.com\n    authorizationUrl: https://vault12.com/core/users/oauth2/authorize\n    tokenUrl: https://vault12.com/core/users/oauth2/token\n\
  \    userinfoUrl: https://vault12.com/core/users/oauth2/user_info\n    registrationUrl: https://vault12.com/core/users/oauth2/register\n    jwksUrl: https://vault12.com/core/users/oauth2/jwks\n    scopes: [openid, profile, email, offline_access]\n    sources: [well-known/vault12-oauth-authorization-server.json]\n  - name: ZaxSessionHandshake\n    type: custom\n    description: >-\n      Anonymous per-session NaCl key establishment on Zax relay nodes:\n      POST /start_session with a random token returns a proof-of-work\n      challenge; POST /verify_session answers it and yields temporary\n      session keys; subsequent POST /command requests are encrypted with\n      the session keys. No long-term credentials or API keys.\n    sources: [https://github.com/vault12/zax]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vault12/refs/heads/main/authentication/vault12-authentication.yml
summary_line: oauth2/session-handshake · 2 schemes
tags:
- Company
- Cryptocurrency
- Security
- Backup
- Inheritance
- Wallets
- Cryptography
- Secret Sharing
- Key Management
---
