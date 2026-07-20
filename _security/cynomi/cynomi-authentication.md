---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cynomi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- implicit
overview: Cynomi secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and implicit flow(s).
provider_name: Cynomi
provider_slug: cynomi
scheme_count: 2
schemes:
- issuer: https://auth.eu.cynomi.com/
  name: Auth0OIDC
  openIdConnectUrl: https://auth.eu.cynomi.com/.well-known/openid-configuration
  sources:
  - well-known/cynomi-openid-configuration.json
  type: openIdConnect
- audience: https://api.prod-eu.eu.cynomi.com/
  flows:
  - authorizationUrl: https://auth.eu.cynomi.com/authorize
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    pkce: true
    tokenUrl: https://auth.eu.cynomi.com/oauth/token
  - deviceAuthorizationUrl: https://auth.eu.cynomi.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.eu.cynomi.com/oauth/token
  jwksUri: https://auth.eu.cynomi.com/.well-known/jwks.json
  name: OAuth2
  revocationUrl: https://auth.eu.cynomi.com/oauth/revoke
  sources:
  - well-known/cynomi-openid-configuration.json
  type: oauth2
  userinfoUrl: https://auth.eu.cynomi.com/userinfo
slug: cynomi-authentication
source_filename: cynomi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://auth.eu.cynomi.com/.well-known/openid-configuration and the\n  dashboard.eu.cynomi.com runtime configuration (Auth0 SPA settings)\ndocs: https://cynomi.com/platform/integrations/public-api/\nsummary:\n  types: [oauth2, openIdConnect]\n  provider: Auth0\n  oauth2_flows: [authorizationCode, deviceCode, implicit]\n  pkce: true\n  token_format: JWT bearer\n  audience: https://api.prod-eu.eu.cynomi.com/\nnotes: >-\n  Cynomi authenticates through an Auth0 tenant (auth.eu.cynomi.com, EU region).\n  The web/dashboard clients use OAuth 2.0 Authorization Code with PKCE (S256) to\n  obtain a JWT access token scoped to the API audience\n  https://api.prod-eu.eu.cynomi.com/. Cynomi's customer-facing Public API (for\n  PSA / ticketing task synchronization) is credentialed from within the platform\n  and its full auth reference is gated behind login; the discovery document below\n  is the authoritative, publicly reachable evidence\
  \ of the OIDC/OAuth2 model.\nschemes:\n- name: Auth0OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.eu.cynomi.com/.well-known/openid-configuration\n  issuer: https://auth.eu.cynomi.com/\n  sources: [well-known/cynomi-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.eu.cynomi.com/authorize\n    tokenUrl: https://auth.eu.cynomi.com/oauth/token\n    pkce: true\n    code_challenge_methods: [S256, plain]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.eu.cynomi.com/oauth/device/code\n    tokenUrl: https://auth.eu.cynomi.com/oauth/token\n  revocationUrl: https://auth.eu.cynomi.com/oauth/revoke\n  userinfoUrl: https://auth.eu.cynomi.com/userinfo\n  jwksUri: https://auth.eu.cynomi.com/.well-known/jwks.json\n  audience: https://api.prod-eu.eu.cynomi.com/\n  sources: [well-known/cynomi-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cynomi/refs/heads/main/authentication/cynomi-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Cybersecurity
- Security
- Compliance
- vCISO
- Risk Management
- GRC
- MSP
- MSSP
- Vulnerability Management
---
