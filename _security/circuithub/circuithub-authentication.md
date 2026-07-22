---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Circuithub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
overview: CircuitHub secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and implicit flow(s).
provider_name: CircuitHub
provider_slug: circuithub
scheme_count: 1
schemes:
- authorization_endpoint: https://auth.circuithub.com/authorize
  code_challenge_methods_supported:
  - S256
  - plain
  device_authorization_endpoint: https://auth.circuithub.com/oauth/device/code
  dpop_signing_alg_values_supported:
  - ES256
  end_session_endpoint: https://auth.circuithub.com/oidc/logout
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - RS256
  - PS256
  - HS256
  issuer: https://auth.circuithub.com/
  jwks_uri: https://auth.circuithub.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://auth.circuithub.com/.well-known/openid-configuration
  provider: Auth0
  revocation_endpoint: https://auth.circuithub.com/oauth/revoke
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  sources:
  - well-known/circuithub-openid-configuration.json
  token_endpoint: https://auth.circuithub.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://auth.circuithub.com/userinfo
slug: circuithub-authentication
source_filename: circuithub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.circuithub.com/.well-known/openid-configuration\nnotes: >-\n  CircuitHub has no public developer API and therefore no OpenAPI security\n  schemes to derive from. End-user authentication for the CircuitHub web\n  application (app.circuithub.com) is handled by an Auth0-hosted OpenID Connect\n  tenant at auth.circuithub.com. The profile below is read verbatim from that\n  tenant's published OIDC discovery document.\nsummary:\n  types: [openIdConnect, oauth2]\n  provider: Auth0\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, implicit]\n  pkce: true\nschemes:\n  - name: OpenIDConnect\n    type: openIdConnect\n    provider: Auth0\n    issuer: https://auth.circuithub.com/\n    openIdConnectUrl: https://auth.circuithub.com/.well-known/openid-configuration\n    authorization_endpoint: https://auth.circuithub.com/authorize\n    token_endpoint: https://auth.circuithub.com/oauth/token\n    userinfo_endpoint:\
  \ https://auth.circuithub.com/userinfo\n    jwks_uri: https://auth.circuithub.com/.well-known/jwks.json\n    device_authorization_endpoint: https://auth.circuithub.com/oauth/device/code\n    revocation_endpoint: https://auth.circuithub.com/oauth/revoke\n    end_session_endpoint: https://auth.circuithub.com/oidc/logout\n    code_challenge_methods_supported: [S256, plain]\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - none\n    id_token_signing_alg_values_supported: [RS256, PS256, HS256]\n    dpop_signing_alg_values_supported: [ES256]\n    scopes_supported:\n      - openid\n      - profile\n      - offline_access\n      - name\n      - given_name\n      - family_name\n\
  \      - nickname\n      - email\n      - email_verified\n      - picture\n      - created_at\n      - identities\n      - phone\n      - address\n    sources: [well-known/circuithub-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuithub/refs/heads/main/authentication/circuithub-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Electronics Manufacturing
- PCB Assembly
- Hardware
- Robotics
- Manufacturing
- Prototyping
- Supply Chain
---
