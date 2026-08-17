---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Atolls Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atolls declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Atolls
provider_slug: atolls
scheme_count: 1
schemes:
- discovery: /.well-known/openid-configuration
  endpoints:
    authorization: '{issuer}/oauth/authorize'
    jwks: '{issuer}/oauth/jwks'
    token: '{issuer}/oauth/token'
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  id: pepper-oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuers:
  - https://www.mydealz.de
  - https://www.hotukdeals.com
  - https://www.dealabs.com
  - https://www.preisjaeger.at
  - https://www.chollometro.com
  - https://www.pepper.pl
  - https://www.promodescuentos.com
  jwks:
    keys: RSA / RS256 signing keys served anonymously
    status: 200
    url: '{issuer}/oauth/jwks'
  name: Pepper community OpenID Connect / OAuth 2.0
  observed:
  - body_shape: RFC 6749 error object with error, error_description and a non-standard `hint`
    content_type: application/json
    probe: POST {issuer}/oauth/token with grant_type=client_credentials and no client_id
    status: 400
  - note: redirects to {issuer}/login — the authorization endpoint is live and gated by an interactive user session.
    probe: GET {issuer}/oauth/authorize?response_type=code&client_id=test
    status: 302
  pkce:
    code_challenge_methods:
    - S256
    - plain
    note: '`plain` is still advertised alongside S256. Current OAuth 2.1 / BCP guidance is S256-only for public clients; advertising `plain` is a downgrade path.'
    supported: true
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - profile
  - email
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: atolls-authentication
source_filename: atolls-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://www.mydealz.de/.well-known/openid-configuration\nnote: >-\n  Atolls publishes no developer portal and no OpenAPI, so there are no OpenAPI\n  securitySchemes to derive from. What it DOES publish — found in this round by\n  probing every owned brand host rather than the corporate host — is a real\n  OpenID Connect / RFC 8414 discovery document on seven Pepper community\n  properties. This artifact is derived from those published discovery documents\n  and from anonymous, unauthenticated calls to the token endpoint. No credentials\n  were used and no access control was bypassed.\nownership: >-\n  The discovery documents self-declare issuer https://www.mydealz.de and\n  https://www.hotukdeals.com — both Atolls-operated Pepper community brands, each of\n  which publishes a security.txt naming atolls.com's disclosure policy and\n  security@atolls.com, and DMARC reports routed to dmarc_rua@atolls.com.\n\nschemes:\n- id: pepper-oidc\n\
  \  type: openIdConnect\n  name: Pepper community OpenID Connect / OAuth 2.0\n  discovery: /.well-known/openid-configuration\n  issuers:\n  - https://www.mydealz.de\n  - https://www.hotukdeals.com\n  - https://www.dealabs.com\n  - https://www.preisjaeger.at\n  - https://www.chollometro.com\n  - https://www.pepper.pl\n  - https://www.promodescuentos.com\n  endpoints:\n    authorization: '{issuer}/oauth/authorize'\n    token: '{issuer}/oauth/token'\n    jwks: '{issuer}/oauth/jwks'\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  response_types_supported:\n  - code\n  subject_types_supported:\n  - public\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n    note: >-\n      `plain` is still advertised alongside S256. Current OAuth 2.1 / BCP guidance is\n      S256-only\
  \ for public clients; advertising `plain` is a downgrade path.\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  jwks:\n    url: '{issuer}/oauth/jwks'\n    status: 200\n    keys: RSA / RS256 signing keys served anonymously\n  observed:\n  - probe: POST {issuer}/oauth/token with grant_type=client_credentials and no client_id\n    status: 400\n    content_type: application/json\n    body_shape: RFC 6749 error object with error, error_description and a non-standard `hint`\n  - probe: GET {issuer}/oauth/authorize?response_type=code&client_id=test\n    status: 302\n    note: redirects to {issuer}/login — the authorization endpoint is live and gated by\n      an interactive user session.\n\ngaps:\n- no userinfo_endpoint is advertised in the discovery document\n- no registration_endpoint (RFC 7591 dynamic client registration) is advertised\n- no /.well-known/oauth-authorization-server (RFC 8414 canonical path) — discovery is\n  only at the OIDC path\n- no /.well-known/oauth-protected-resource\
  \ (RFC 9728), so a client cannot discover\n  which resource server these tokens are for\n- no public client registration path, developer portal, or documented API the issued\n  tokens are meant to call\n\ndocs: null\ndocs_note: >-\n  No authentication documentation is published. atolls.com/developers,\n  mydealz.de/developers and mydealz.de/api-docs all miss (404, or a soft-200 catch-all\n  on hotukdeals.com), and api./developer./docs.atolls.com do not resolve in DNS.\n  The OIDC discovery document is currently the only machine-readable statement Atolls\n  makes about authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atolls/refs/heads/main/authentication/atolls-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer
- E-Commerce
- Affiliate Marketing
- Cashback
- Coupons
- Shopping
- Retail
- Identity
- OpenID Connect
---
