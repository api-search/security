---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Niteshift Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- clientCredentials
- refreshToken
overview: Niteshift secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, clientCredentials, and refreshToken flow(s).
provider_name: Niteshift
provider_slug: niteshift
scheme_count: 2
schemes:
- authorization_endpoint: https://auth.niteshift.dev/oauth2/authorize
  code_challenge_methods_supported:
  - S256
  device_authorization_endpoint: https://auth.niteshift.dev/oauth2/device_authorization
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://auth.niteshift.dev/oauth2/introspection
  issuer: https://auth.niteshift.dev
  jwks_uri: https://auth.niteshift.dev/oauth2/jwks
  name: OAuth2
  registration_endpoint: https://auth.niteshift.dev/oauth2/register
  sources:
  - well-known/niteshift-oauth-authorization-server.json
  token_endpoint: https://auth.niteshift.dev/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
  userinfo_endpoint: https://auth.niteshift.dev/oauth2/userinfo
- id_token_signing_alg_values_supported:
  - RS256
  name: OpenIDConnect
  openIdConnectUrl: https://auth.niteshift.dev/.well-known/openid-configuration
  sources:
  - well-known/niteshift-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: niteshift-authentication
source_filename: niteshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://niteshift.dev/.well-known/oauth-authorization-server\ndocs: https://auth.niteshift.dev/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, deviceCode, clientCredentials, refreshToken]\n  pkce: [S256]\n  oidc: true\nschemes:\n  - name: OAuth2\n    type: oauth2\n    issuer: https://auth.niteshift.dev\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n    authorization_endpoint: https://auth.niteshift.dev/oauth2/authorize\n    token_endpoint: https://auth.niteshift.dev/oauth2/token\n    device_authorization_endpoint: https://auth.niteshift.dev/oauth2/device_authorization\n    introspection_endpoint: https://auth.niteshift.dev/oauth2/introspection\n    registration_endpoint: https://auth.niteshift.dev/oauth2/register\n    userinfo_endpoint: https://auth.niteshift.dev/oauth2/userinfo\n\
  \    jwks_uri: https://auth.niteshift.dev/oauth2/jwks\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n    sources: [well-known/niteshift-oauth-authorization-server.json]\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://auth.niteshift.dev/.well-known/openid-configuration\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    sources: [well-known/niteshift-openid-configuration.json]\nnotes: >-\n  Auth profile derived from Niteshift's published RFC 8414 authorization-server\n  metadata and OIDC discovery document (no provider OpenAPI is published).\n  Supports Dynamic Client Registration (RFC 7591) and the OAuth 2.0 Device\n  Authorization Grant, consistent with a CLI / coding-agent client model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niteshift/refs/heads/main/authentication/niteshift-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Infrastructure
- Coding Agents
- AI Agents
- Developer Tools
- Cloud Development Environments
- DevOps
- Automation
---
