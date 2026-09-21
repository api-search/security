---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Avery Dennison Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avery Dennison declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Avery Dennison
provider_slug: avery-dennison
scheme_count: 2
schemes:
- api_scopes: undocumented
  audience: https://open.atma.io
  dynamic_client_registration: https://login.atma.io/oidc/register
  evidence:
  - status: 200
    url: https://login.atma.io/.well-known/openid-configuration
  - note: redirects to https://login.atma.io/authorize?...&audience=https%3A%2F%2Fopen.atma.io&code_challenge_method=S256
    status: 302
    url: https://docs.atma.io/
  flows:
    authorizationCode:
      authorizationUrl: https://login.atma.io/authorize
      pkce: S256
      refreshUrl: https://login.atma.io/oauth/token
      tokenUrl: https://login.atma.io/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://login.atma.io/oauth/device/code
      tokenUrl: https://login.atma.io/oauth/token
  identity_scopes:
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
  issuer: https://login.atma.io/
  jwks_uri: https://login.atma.io/.well-known/jwks.json
  name: atma-oauth2
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
- evidence:
  - status: 302
    url: https://developer.averydennison.com/developers/
  issuer: https://averydennison.okta.com/oauth2/v1
  name: developer-portal-okta
  note: developer.averydennison.com is a Vouch-proxied portal whose every path 302s to an Okta authorization request (scope openid email). This gates the portal, not an API; it is recorded so the wall is on record.
  type: openIdConnect
slug: avery-dennison-authentication
source_filename: avery-dennison-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: https://login.atma.io/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  The atma.io connected product cloud API (audience https://open.atma.io) is gated by OAuth 2.0 /\n  OpenID Connect issued from an Auth0 tenant on the provider's own custom domain, login.atma.io.\n  The documentation portal docs.atma.io itself redirects anonymous visitors into that authorization\n  flow (authorization code + PKCE S256, scopes openid profile email offline_access), so no public\n  authentication guide, API-key scheme or scope reference could be read. The profile below is what\n  the identity provider publishes about itself; API-level scopes for open.atma.io are undocumented.\nschemes:\n- name: atma-oauth2\n  type: oauth2\n  issuer: https://login.atma.io/\n  flows:\n    authorizationCode:\n      authorizationUrl: https://login.atma.io/authorize\n      tokenUrl: https://login.atma.io/oauth/token\n      refreshUrl: https://login.atma.io/oauth/token\n\
  \      pkce: S256\n    deviceCode:\n      deviceAuthorizationUrl: https://login.atma.io/oauth/device/code\n      tokenUrl: https://login.atma.io/oauth/token\n  audience: https://open.atma.io\n  identity_scopes: [openid, profile, offline_access, name, given_name, family_name, nickname, email, email_verified, picture, created_at, identities, phone, address]\n  api_scopes: undocumented\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  jwks_uri: https://login.atma.io/.well-known/jwks.json\n  dynamic_client_registration: https://login.atma.io/oidc/register\n  evidence:\n  - url: https://login.atma.io/.well-known/openid-configuration\n    status: 200\n  - url: https://docs.atma.io/\n    status: 302\n    note: redirects to https://login.atma.io/authorize?...&audience=https%3A%2F%2Fopen.atma.io&code_challenge_method=S256\n- name: developer-portal-okta\n  type: openIdConnect\n  issuer: https://averydennison.okta.com/oauth2/v1\n  note: >-\n    developer.averydennison.com\
  \ is a Vouch-proxied portal whose every path 302s to an Okta\n    authorization request (scope openid email). This gates the portal, not an API; it is recorded\n    so the wall is on record.\n  evidence:\n  - url: https://developer.averydennison.com/developers/\n    status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avery-dennison/refs/heads/main/authentication/avery-dennison-authentication.yml
summary_line: 2 schemes
tags:
- Fortune 500
- IoT
- RFID
- Labels
- Supply Chain
- Manufacturing
- Digital Product Passport
---
