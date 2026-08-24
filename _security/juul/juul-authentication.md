---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Juul Authentication
name_suffix: Authentication
oauth_flows: []
overview: JUUL declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: JUUL
provider_slug: juul
scheme_count: 1
schemes:
- claims:
  - exp
  - iat
  - iss
  - locale
  - sub
  description: OAuth 2.0 authorization server advertised at the OIDC discovery path. The metadata is RFC 8414-shaped (authorization/token/revocation endpoints, grant types, scopes) but omits the OIDC-required jwks_uri and id_token_signing_alg_values_supported, so it is an OAuth 2.0 authorization server publishing at the OpenID Connect discovery URL rather than a certified OpenID Provider.
  flows:
    authorization_code:
      authorization_url: https://www.juul.com/sso
      refresh_url: https://www.juul.com/oauth/token
      scopes:
        conx_web: null
        keychain: null
        keychain-force-rebuild: null
        mobileapp: null
      token_url: https://www.juul.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: juul-oauth2
  response_types:
  - code
  - token
  - password
  - none
  revocation_url: https://www.juul.com/oauth/revoke
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
  userinfo_url: https://www.juul.com/oauth/token/info
slug: juul-authentication
source_filename: juul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://www.juul.com/.well-known/openid-configuration\nnote: >-\n  JUUL Labs publishes no public API and no developer authentication documentation. This profile is\n  derived entirely from the OAuth 2.0 / OIDC discovery document JUUL serves anonymously from its own\n  consumer commerce host — it describes JUUL's FIRST-PARTY sign-in for juul.com and the JUUL mobile\n  app, not a third-party developer program. There is no public client registration, no documented\n  scope reference, and no published token issuance path for outside integrators.\naudience: first-party\npublic_developer_program: false\nissuer: https://www.juul.com\nschemes:\n- id: juul-oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization server advertised at the OIDC discovery path. The metadata is\n    RFC 8414-shaped (authorization/token/revocation endpoints, grant types, scopes) but omits the\n    OIDC-required jwks_uri and id_token_signing_alg_values_supported,\
  \ so it is an OAuth 2.0\n    authorization server publishing at the OpenID Connect discovery URL rather than a certified\n    OpenID Provider.\n  flows:\n    authorization_code:\n      authorization_url: https://www.juul.com/sso\n      token_url: https://www.juul.com/oauth/token\n      refresh_url: https://www.juul.com/oauth/token\n      scopes:\n        conx_web: null\n        mobileapp: null\n        keychain: null\n        keychain-force-rebuild: null\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  - token\n  - password\n  - none\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  userinfo_url: https://www.juul.com/oauth/token/info\n  revocation_url: https://www.juul.com/oauth/revoke\n  subject_types:\n  - public\n  claims:\n  - exp\n  - iat\n  - iss\n  - locale\n  - sub\nendpoint_reachability:\n  note: >-\n    The authorization, token, userinfo and revocation\
  \ endpoints named in the metadata all sit behind\n    AWS WAF. An anonymous GET to each returns HTTP 202 with an empty body and the header\n    x-amzn-waf-action: challenge, so their live behaviour could not be observed without solving a\n    bot challenge, which this pipeline does not do.\n  probes:\n  - url: https://www.juul.com/sso\n    status: 202\n  - url: https://www.juul.com/oauth/token\n    status: 202\n  - url: https://www.juul.com/oauth/token/info\n    status: 202\n  - url: https://www.juul.com/oauth/revoke\n    status: 202\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juul/refs/heads/main/authentication/juul-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consumer Products
- Nicotine
- Vaping
- Hardware
- Consumer Electronics
- Bluetooth Low Energy
- Open Source
- Kotlin Multiplatform
- Regulated Industry
---
