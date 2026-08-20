---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Thought Machine Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- refreshToken
- deviceCode
overview: Thought Machine secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, refreshToken, and deviceCode flow(s).
provider_name: Thought Machine
provider_slug: thought-machine
scheme_count: 1
schemes:
- backchannel_logout_supported: true
  code_challenge_methods:
  - plain
  - S256
  endpoints:
    authorization: https://auth.thoughtmachine.net/application/o/authorize/
    device_authorization: https://auth.thoughtmachine.net/application/o/device/
    end_session: https://auth.thoughtmachine.net/application/o/vault-portal/end-session/
    introspection: https://auth.thoughtmachine.net/application/o/introspect/
    jwks: https://auth.thoughtmachine.net/application/o/vault-portal/jwks/
    revocation: https://auth.thoughtmachine.net/application/o/revoke/
    token: https://auth.thoughtmachine.net/application/o/token/
    userinfo: https://auth.thoughtmachine.net/application/o/userinfo/
  frontchannel_logout_supported: true
  grant_types:
  - authorization_code
  - refresh_token
  - implicit
  - client_credentials
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  issuer: https://auth.thoughtmachine.net/application/o/vault-portal/
  name: vault-portal-oidc
  openIdConnectUrl: https://auth.thoughtmachine.net/application/o/vault-portal/.well-known/openid-configuration
  provider: Authentik (goauthentik.io)
  response_types:
  - code
  - id_token
  - id_token token
  - code token
  - code id_token
  - code id_token token
  sources:
  - well-known/thought-machine-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
slug: thought-machine-authentication
source_filename: thought-machine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://auth.thoughtmachine.net/application/o/vault-portal/.well-known/openid-configuration\ndocs: https://docs.thoughtmachine.net/\nx-note: >-\n  Thought Machine publishes no public OpenAPI, so no securitySchemes could be derived. What is\n  anonymously observable is the OpenID Connect discovery document for the Vault portal identity\n  provider (Authentik), captured verbatim at\n  well-known/thought-machine-openid-configuration.json. The Vault Core and Vault Payments API\n  authentication model itself is documented behind the partner login at docs.thoughtmachine.net\n  and was NOT observable; nothing about it is asserted here.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - refreshToken\n  - deviceCode\n  pkce: true\n  scope: vault developer/enablement portal SSO (not the Vault Core / Vault Payments data APIs)\nschemes:\n- name:\
  \ vault-portal-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.thoughtmachine.net/application/o/vault-portal/.well-known/openid-configuration\n  issuer: https://auth.thoughtmachine.net/application/o/vault-portal/\n  provider: Authentik (goauthentik.io)\n  endpoints:\n    authorization: https://auth.thoughtmachine.net/application/o/authorize/\n    token: https://auth.thoughtmachine.net/application/o/token/\n    userinfo: https://auth.thoughtmachine.net/application/o/userinfo/\n    introspection: https://auth.thoughtmachine.net/application/o/introspect/\n    revocation: https://auth.thoughtmachine.net/application/o/revoke/\n    device_authorization: https://auth.thoughtmachine.net/application/o/device/\n    end_session: https://auth.thoughtmachine.net/application/o/vault-portal/end-session/\n    jwks: https://auth.thoughtmachine.net/application/o/vault-portal/jwks/\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - implicit\n  - client_credentials\n  - password\n\
  \  - urn:ietf:params:oauth:grant-type:device_code\n  response_types:\n  - code\n  - id_token\n  - id_token token\n  - code token\n  - code id_token\n  - code id_token token\n  code_challenge_methods:\n  - plain\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  backchannel_logout_supported: true\n  frontchannel_logout_supported: true\n  sources:\n  - well-known/thought-machine-openid-configuration.json\ngated:\n- surface: Vault Core Core API / Posting API / Contracts API\n  auth_documented_at: https://docs.thoughtmachine.net/\n  observable: false\n  reason: documentation host requires partner SSO login\n- surface: Vault Payments REST and streaming APIs\n  auth_documented_at: https://docs.thoughtmachine.net/\n  observable: false\n  reason: documentation host requires partner SSO login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thought-machine/refs/heads/main/authentication/thought-machine-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Banking
- Core Banking
- Financial-Services
- Payments
- Cloud-Native
- Smart Contracts
- ISO 20022
- Ledger
- Fintech
- United Kingdom
---
