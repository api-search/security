---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Soundboks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Soundboks secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Soundboks
provider_slug: soundboks
scheme_count: 2
schemes:
- id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/6044516441
  name: openIdConnect
  openIdConnectUrl: https://soundboks.com/.well-known/openid-configuration
  sources:
  - well-known/soundboks-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://us-account.soundboks.com/authentication/oauth/authorize
    codeChallengeMethods:
    - S256
    endSessionUrl: https://us-account.soundboks.com/authentication/logout
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    jwksUrl: https://us-account.soundboks.com/authentication/.well-known/jwks.json
    tokenUrl: https://us-account.soundboks.com/authentication/oauth/token
  name: oauth2
  sources:
  - well-known/soundboks-oauth-authorization-server.json
  type: oauth2
slug: soundboks-authentication
source_filename: soundboks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://soundboks.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Auth profile derived from the live OIDC/OAuth discovery documents on the\n  soundboks.com store domain. This is the Shopify Customer Accounts platform\n  (issuer https://shopify.com/authentication/6044516441) configured for Soundboks,\n  not a Soundboks-authored API. No first-party developer API is published.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/6044516441\n  openIdConnectUrl: https://soundboks.com/.well-known/openid-configuration\n  id_token_signing_alg: RS256\n  sources:\n  - well-known/soundboks-openid-configuration.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://us-account.soundboks.com/authentication/oauth/authorize\n    tokenUrl: https://us-account.soundboks.com/authentication/oauth/token\n    endSessionUrl: https://us-account.soundboks.com/authentication/logout\n    jwksUrl: https://us-account.soundboks.com/authentication/.well-known/jwks.json\n    codeChallengeMethods:\n    - S256\n    grantTypes:\n    - authorization_code\n    - refresh_token\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  sources:\n  - well-known/soundboks-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundboks/refs/heads/main/authentication/soundboks-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Consumer Electronics
- Audio
- Bluetooth Speakers
- Hardware
- E-commerce
- Shopify
- Direct-to-Consumer
---
