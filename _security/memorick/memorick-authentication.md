---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Memorick Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- personalAccessToken
overview: Memorick secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and personalAccessToken flow(s).
provider_name: Memorick
provider_slug: memorick
scheme_count: 4
schemes:
- endpoints:
    authorize: https://memorick.com/oauth/authorize
    clients: https://memorick.com/oauth/clients
    personal_access_tokens: https://memorick.com/oauth/personal-access-tokens
    scopes: https://memorick.com/oauth/scopes
    token: https://memorick.com/oauth/token
    token_refresh: https://memorick.com/oauth/token/refresh
  flows:
  - authorizationUrl: https://memorick.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://memorick.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://memorick.com/oauth/token/refresh
  name: OAuth2 (Laravel Passport)
  sources:
  - live-route-manifest
  type: oauth2
- description: Laravel Passport personal access tokens issued from the account UI.
  name: Personal Access Tokens
  scheme: bearer
  sources:
  - live-route-manifest
  type: http
- description: Cookie/session authentication for the first-party single-page application, bootstrapped via GET /sanctum/csrf-cookie.
  name: Sanctum (first-party session)
  scheme: cookie
  sources:
  - live-route-manifest
  type: http
- description: Optional TOTP two-factor challenge (two-factor-challenge, two-factor-qr-code, two-factor-recovery-codes) layered on session auth.
  name: Two-factor authentication (Laravel Fortify)
  scheme: session
  sources:
  - live-route-manifest
  type: http
slug: memorick-authentication
source_filename: memorick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://memorick.com\nnotes: >-\n  Memorick publishes no OpenAPI/Swagger definition, so this profile is derived from\n  the live, observable authorization surface exposed by the application (a Laravel\n  app using Passport for OAuth2, Sanctum for first-party session auth, and Fortify\n  for two-factor). Endpoint paths were confirmed against the live host; the OAuth2\n  scope catalog is not publicly published and is therefore not enumerated here (no\n  fabrication).\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - personalAccessToken\nschemes:\n- name: OAuth2 (Laravel Passport)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://memorick.com/oauth/authorize\n    tokenUrl: https://memorick.com/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://memorick.com/oauth/token/refresh\n  endpoints:\n    authorize: https://memorick.com/oauth/authorize\n\
  \    token: https://memorick.com/oauth/token\n    token_refresh: https://memorick.com/oauth/token/refresh\n    clients: https://memorick.com/oauth/clients\n    scopes: https://memorick.com/oauth/scopes\n    personal_access_tokens: https://memorick.com/oauth/personal-access-tokens\n  sources:\n  - live-route-manifest\n- name: Personal Access Tokens\n  type: http\n  scheme: bearer\n  description: Laravel Passport personal access tokens issued from the account UI.\n  sources:\n  - live-route-manifest\n- name: Sanctum (first-party session)\n  type: http\n  scheme: cookie\n  description: >-\n    Cookie/session authentication for the first-party single-page application,\n    bootstrapped via GET /sanctum/csrf-cookie.\n  sources:\n  - live-route-manifest\n- name: Two-factor authentication (Laravel Fortify)\n  type: http\n  scheme: session\n  description: >-\n    Optional TOTP two-factor challenge (two-factor-challenge, two-factor-qr-code,\n    two-factor-recovery-codes) layered on session auth.\n\
  \  sources:\n  - live-route-manifest\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memorick/refs/heads/main/authentication/memorick-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Company
- Photography
- Booking
- Marketplace
- Travel
- Photographers
- OAuth
- Laravel
---
