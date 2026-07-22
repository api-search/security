---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Black Ore Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- deviceCode
overview: Black Ore secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and deviceCode flow(s).
provider_name: Black Ore
provider_slug: black-ore
scheme_count: 2
schemes:
- issuer: https://auth.blackore.ai/
  name: OpenIDConnect
  openIdConnectUrl: https://auth.blackore.ai/.well-known/openid-configuration
  sources:
  - well-known/black-ore-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://auth.blackore.ai/authorize
  deviceAuthorizationUrl: https://auth.blackore.ai/oauth/device/code
  jwksUrl: https://auth.blackore.ai/.well-known/jwks.json
  name: OAuth2
  registrationUrl: https://auth.blackore.ai/oidc/register
  revocationUrl: https://auth.blackore.ai/oauth/revoke
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
  - well-known/black-ore-oauth-authorization-server.json
  tokenUrl: https://auth.blackore.ai/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
slug: black-ore-authentication
source_filename: black-ore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.blackore.ai/.well-known/openid-configuration\n# No public OpenAPI is available for Black Ore; this auth profile is captured from\n# the live OIDC/OAuth 2.0 discovery documents served by the platform's identity\n# tenant (Auth0-hosted) at auth.blackore.ai. Platform sign-in and any customer\n# API integration are gated through this tenant.\ndocs: https://blackore.ai/security\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, implicit, deviceCode]\n  pkce: [S256, plain]\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.blackore.ai/.well-known/openid-configuration\n  issuer: https://auth.blackore.ai/\n  sources: [well-known/black-ore-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  authorizationUrl: https://auth.blackore.ai/authorize\n  tokenUrl: https://auth.blackore.ai/oauth/token\n  deviceAuthorizationUrl: https://auth.blackore.ai/oauth/device/code\n\
  \  revocationUrl: https://auth.blackore.ai/oauth/revoke\n  registrationUrl: https://auth.blackore.ai/oidc/register\n  jwksUrl: https://auth.blackore.ai/.well-known/jwks.json\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  scopes_supported: [openid, profile, offline_access, name, given_name, family_name,\n    nickname, email, email_verified, picture, created_at, identities, phone, address]\n  sources: [well-known/black-ore-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-ore/refs/heads/main/authentication/black-ore-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Tax
- Accounting
- Artificial Intelligence
- Financial Services
- Automation
- Machine Learning
---
