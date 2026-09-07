---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 247 Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- clientCredentials
- deviceCode
overview: '[24]7.ai secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, clientCredentials, and deviceCode flow(s).'
provider_name: '[24]7.ai'
provider_slug: 247-ai
scheme_count: 2
schemes:
- code_challenge_methods:
  - S256
  dynamic_client_registration: true
  endpoints:
    authorization: https://login.247.ai/oauth2/v1/authorize
    end_session: https://login.247.ai/oauth2/v1/logout
    jwks: https://login.247.ai/oauth2/v1/keys
    registration: https://login.247.ai/oauth2/v1/clients
    token: https://login.247.ai/oauth2/v1/token
    userinfo: https://login.247.ai/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://login.247.ai
  name: '[24]7 Engagement Cloud SSO (OpenID Connect)'
  openIdConnectUrl: https://login.247.ai/.well-known/openid-configuration
  response_types:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  sources:
  - well-known/247-ai-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- dpop_signing_algs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://login.247.ai/oauth2/v1/authorize
    introspection: https://login.247.ai/oauth2/v1/introspect
    revocation: https://login.247.ai/oauth2/v1/revoke
    token: https://login.247.ai/oauth2/v1/token
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://login.247.ai
  metadata: https://login.247.ai/.well-known/oauth-authorization-server
  name: '[24]7 Engagement Cloud org authorization server (OAuth 2.0)'
  scopes_ref: scopes/247-ai-scopes.yml
  sources:
  - well-known/247-ai-oauth-authorization-server.json
  type: oauth2
slug: 247-ai-authentication
source_filename: 247-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://login.247.ai/.well-known/openid-configuration\ndocs: https://www.247.ai/product-login-and-support/\nnote: >-\n  [24]7.ai publishes no OpenAPI, so there are no securitySchemes to derive from\n  (0-working/derive-authentication.py has no spec input for this provider). What IS\n  machine-readable is the identity surface: login.247.ai — the Okta-hosted [24]7 Engagement\n  Cloud SSO tenant — serves live OpenID Connect discovery (OIDC Discovery 1.0) and OAuth 2.0\n  authorization server metadata (RFC 8414). Both were fetched anonymously and saved verbatim\n  under well-known/. This describes how a HUMAN or a registered client signs in to the\n  Engagement Cloud, not how a product API is authenticated; [24]7.ai documents no public API\n  authentication because it publishes no public API reference.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, implicit, refreshToken, password, clientCredentials,\
  \ deviceCode]\n  pkce: [S256]\n  api_key_in: []\nschemes:\n- name: '[24]7 Engagement Cloud SSO (OpenID Connect)'\n  type: openIdConnect\n  openIdConnectUrl: https://login.247.ai/.well-known/openid-configuration\n  issuer: https://login.247.ai\n  sources: [well-known/247-ai-openid-configuration.json]\n  endpoints:\n    authorization: https://login.247.ai/oauth2/v1/authorize\n    token: https://login.247.ai/oauth2/v1/token\n    userinfo: https://login.247.ai/oauth2/v1/userinfo\n    jwks: https://login.247.ai/oauth2/v1/keys\n    registration: https://login.247.ai/oauth2/v1/clients\n    end_session: https://login.247.ai/oauth2/v1/logout\n  response_types: [code, id_token, 'code id_token', 'code token', 'id_token token', 'code id_token token']\n  grant_types: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n  code_challenge_methods:\
  \ [S256]\n  dynamic_client_registration: true\n- name: '[24]7 Engagement Cloud org authorization server (OAuth 2.0)'\n  type: oauth2\n  metadata: https://login.247.ai/.well-known/oauth-authorization-server\n  issuer: https://login.247.ai\n  sources: [well-known/247-ai-oauth-authorization-server.json]\n  endpoints:\n    authorization: https://login.247.ai/oauth2/v1/authorize\n    token: https://login.247.ai/oauth2/v1/token\n    introspection: https://login.247.ai/oauth2/v1/introspect\n    revocation: https://login.247.ai/oauth2/v1/revoke\n  grant_types: [authorization_code, implicit, refresh_token, password, client_credentials, 'urn:ietf:params:oauth:grant-type:device_code']\n  dpop_signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512]\n  scopes_ref: scopes/247-ai-scopes.yml\nx-evidence:\n- {url: 'https://login.247.ai/.well-known/openid-configuration', http_status: 200, content_type: application/json, fetched: '2026-09-05'}\n- {url: 'https://login.247.ai/.well-known/oauth-authorization-server',\
  \ http_status: 200, content_type: application/json, fetched: '2026-09-05'}\n- {url: 'https://www.247.ai/llms.txt', http_status: 200, note: 'names no developer portal, API reference or authentication guide'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/247-ai/refs/heads/main/authentication/247-ai-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Customer Experience
- Conversational AI
- Contact Center
- Customer Service
- Chatbots
- CCaaS
- Artificial Intelligence
- Interaction Analytics
- Business Process Outsourcing
---
