---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Impartner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- deviceCode
overview: Impartner secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, and deviceCode flow(s).
provider_name: Impartner
provider_slug: impartner
scheme_count: 3
schemes:
- authorization_endpoint: https://login.impartner.com/authorize
  code_challenge_methods:
  - S256
  - plain
  device_authorization_endpoint: https://login.impartner.com/oauth/device/code
  issuer: https://login.impartner.com/
  jwks_uri: https://login.impartner.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://login.impartner.com/.well-known/openid-configuration
  revocation_endpoint: https://login.impartner.com/oauth/revoke
  sources:
  - well-known/impartner-openid-configuration.json
  token_endpoint: https://login.impartner.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://login.impartner.com/userinfo
- flows:
  - authorizationUrl: https://login.impartner.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.impartner.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.impartner.com/oauth/token
  name: OAuth2
  sources:
  - well-known/impartner-openid-configuration.json
  type: oauth2
- in: header
  name: ApiKey
  note: The Impartner Objects API (v1, base https://prod.impartner.live) is also accessed with an API key issued per-tenant; per Impartner integration docs the key is obtained by contacting an Impartner representative. Third-party connectors (Cortex XSOAR, Tray) authenticate with this key.
  sources:
  - https://xsoar.pan.dev/docs/reference/integrations/impartner
  type: apiKey
slug: impartner-authentication
source_filename: impartner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://login.impartner.com/.well-known/openid-configuration\ndocs: https://developer.impartner.com\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  oauth2_flows: [authorizationCode, clientCredentials, password, deviceCode]\n  api_key_in: [header]\n  identity_provider: Auth0 (tenant impartner.auth0.com, public issuer https://login.impartner.com/)\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://login.impartner.com/.well-known/openid-configuration\n  issuer: https://login.impartner.com/\n  authorization_endpoint: https://login.impartner.com/authorize\n  token_endpoint: https://login.impartner.com/oauth/token\n  userinfo_endpoint: https://login.impartner.com/userinfo\n  jwks_uri: https://login.impartner.com/.well-known/jwks.json\n  revocation_endpoint: https://login.impartner.com/oauth/revoke\n  device_authorization_endpoint: https://login.impartner.com/oauth/device/code\n  token_endpoint_auth_methods:\
  \ [client_secret_basic, client_secret_post, private_key_jwt, none]\n  code_challenge_methods: [S256, plain]\n  sources: [well-known/impartner-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.impartner.com/authorize\n    tokenUrl: https://login.impartner.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.impartner.com/oauth/token\n  sources: [well-known/impartner-openid-configuration.json]\n- name: ApiKey\n  type: apiKey\n  in: header\n  note: >-\n    The Impartner Objects API (v1, base https://prod.impartner.live) is also accessed with an API\n    key issued per-tenant; per Impartner integration docs the key is obtained by contacting an\n    Impartner representative. Third-party connectors (Cortex XSOAR, Tray) authenticate with this key.\n  sources: [https://xsoar.pan.dev/docs/reference/integrations/impartner]\nnotes:\n- The platform SSO / app login is OAuth2 + OIDC on an Auth0\
  \ tenant (login.impartner.com).\n- The programmatic Objects API uses a tenant API key; SOAP and REST are both offered.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impartner/refs/heads/main/authentication/impartner-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- SaaS
- Partner Relationship Management
- PRM
- Channel Management
- Partner Ecosystem
- Through-Channel Marketing
- Sales
- CRM
---
