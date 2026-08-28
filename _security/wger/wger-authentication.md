---
api_key_in:
- cookie
- header
api_specs:
- filename: wger-openapi.yml
  format: yaml
  label: Wger REST API v2
  slug: wger-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wger/refs/heads/main/openapi/wger-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wger Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wger secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wger
provider_slug: wger
scheme_count: 5
schemes:
- description: Permanent personal API key. Minted from the web UI at /en/user/api-key (User settings -> API key). Intended for personal scripts and long-running integrations; shown once.
  docs: https://wger.readthedocs.io/en/latest/api/api.html
  in: header
  name: tokenAuth
  parameter: Authorization
  prefix: 'Token '
  sources:
  - openapi/wger-openapi.yml
  - https://wger.readthedocs.io/en/latest/api/api.html
  type: apiKey
- bearerFormat: JWT
  description: Short-lived JWT access token (10 minutes in the Docker default) paired with a long-lived refresh token (120 days). Lifetimes are configurable per instance via ACCESS_TOKEN_LIFETIME / REFRESH_TOKEN_LIFETIME. Recommended mechanism for apps.
  docs: https://wger.readthedocs.io/en/latest/api/api.html
  name: jwtAuth
  rotation: Refresh rotates both tokens; the previous refresh token is blacklisted immediately.
  scheme: bearer
  sources:
  - openapi/wger-openapi.yml
  - https://wger.readthedocs.io/en/latest/api/api.html
  token_endpoints:
    refresh: POST /api/v2/token/refresh
    verify: POST /api/v2/token/verify
  type: http
- bearerFormat: JWT
  description: Access token issued by the django-allauth headless endpoints. wger deliberately has no credentials-to-JWT endpoint because it would bypass 2FA; a refresh token comes from POST /allauth/app/v1/auth/login (with a partial-login + X-Session-Token / requires_mfa step through POST /allauth/app/v1/auth/2fa/authenticate when 2FA is enabled), or from the web API key page.
  name: headlessJwtAuth
  scheme: bearer
  sources:
  - openapi/wger-openapi.yml
  - https://wger.readthedocs.io/en/latest/api/api.html
  type: http
  upstream_spec: https://docs.allauth.org/en/latest/headless/openapi-specification/
- description: wger can act as an OAuth2/OIDC provider itself (django-oauth-toolkit), so other applications can let their users sign in with a wger account and call the API on their behalf. Off by default unless the instance configures it; enabled on wger.de.
  device_authorization_endpoint: https://wger.de/identity/o/api/device/code
  discovery: https://wger.de/.well-known/openid-configuration
  docs: https://wger.readthedocs.io/en/latest/administration/oauth2_provider.html
  flows:
  - authorizationUrl: https://wger.de/identity/o/authorize
    flow: authorizationCode
    pkce: S256
    scopes: 2
    tokenUrl: https://wger.de/identity/o/api/token
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  jwks_uri: https://wger.de/.well-known/jwks.json
  name: oidcAuth
  revocation_endpoint: https://wger.de/identity/o/api/revoke
  sources:
  - openapi/wger-openapi.yml
  - https://wger.de/.well-known/openid-configuration
  type: oauth2
  userinfo_endpoint: https://wger.de/identity/o/api/userinfo
- description: The Django session cookie a logged-in browser already carries. Used by wger's own web UI and by the browsable API.
  in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/wger-openapi.yml
  type: apiKey
slug: wger-authentication
source_filename: wger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://wger.readthedocs.io/en/latest/api/api.html\ndocs: https://wger.readthedocs.io/en/latest/api/api.html\nspec: openapi/wger-openapi.yml\nnote: >-\n  Derived from the securitySchemes in openapi/wger-openapi.yml (fetched from\n  https://wger.de/api/v2/schema) and upgraded from the wger \"Using the API\"\n  documentation. The API tries credentials in the order Token -> Bearer JWT ->\n  session cookie. System-wide reference data (exercises, ingredients, units,\n  muscles, equipment) is readable with no credential at all.\nanonymous_access:\n  supported: true\n  scope: >-\n    System-wide/community data: /api/v2/exercise*, /api/v2/ingredient*,\n    /api/v2/muscle/, /api/v2/equipment/, /api/v2/exercisecategory/,\n    /api/v2/language/, /api/v2/license/, /api/v2/public-templates/ and the\n    setting-*unit reference endpoints.\n  source: https://wger.readthedocs.io/en/latest/api/api.html\nsummary:\n  types:\n    - apiKey\n  \
  \  - http\n    - oauth2\n  api_key_in:\n    - cookie\n    - header\n  oauth2_flows:\n    - authorizationCode\nschemes:\n  - name: tokenAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    prefix: 'Token '\n    description: >-\n      Permanent personal API key. Minted from the web UI at\n      /en/user/api-key (User settings -> API key). Intended for personal\n      scripts and long-running integrations; shown once.\n    docs: https://wger.readthedocs.io/en/latest/api/api.html\n    sources:\n      - openapi/wger-openapi.yml\n      - https://wger.readthedocs.io/en/latest/api/api.html\n  - name: jwtAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Short-lived JWT access token (10 minutes in the Docker default) paired\n      with a long-lived refresh token (120 days). Lifetimes are configurable\n      per instance via ACCESS_TOKEN_LIFETIME / REFRESH_TOKEN_LIFETIME.\n      Recommended mechanism for apps.\n    token_endpoints:\n\
  \      refresh: POST /api/v2/token/refresh\n      verify: POST /api/v2/token/verify\n    rotation: >-\n      Refresh rotates both tokens; the previous refresh token is blacklisted\n      immediately.\n    docs: https://wger.readthedocs.io/en/latest/api/api.html\n    sources:\n      - openapi/wger-openapi.yml\n      - https://wger.readthedocs.io/en/latest/api/api.html\n  - name: headlessJwtAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Access token issued by the django-allauth headless endpoints. wger\n      deliberately has no credentials-to-JWT endpoint because it would bypass\n      2FA; a refresh token comes from POST /allauth/app/v1/auth/login (with a\n      partial-login + X-Session-Token / requires_mfa step through\n      POST /allauth/app/v1/auth/2fa/authenticate when 2FA is enabled), or from\n      the web API key page.\n    upstream_spec: https://docs.allauth.org/en/latest/headless/openapi-specification/\n    sources:\n      - openapi/wger-openapi.yml\n\
  \      - https://wger.readthedocs.io/en/latest/api/api.html\n  - name: oidcAuth\n    type: oauth2\n    description: >-\n      wger can act as an OAuth2/OIDC provider itself (django-oauth-toolkit), so\n      other applications can let their users sign in with a wger account and\n      call the API on their behalf. Off by default unless the instance\n      configures it; enabled on wger.de.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://wger.de/identity/o/authorize\n        tokenUrl: https://wger.de/identity/o/api/token\n        scopes: 2\n        pkce: S256\n    discovery: https://wger.de/.well-known/openid-configuration\n    jwks_uri: https://wger.de/.well-known/jwks.json\n    userinfo_endpoint: https://wger.de/identity/o/api/userinfo\n    revocation_endpoint: https://wger.de/identity/o/api/revoke\n    device_authorization_endpoint: https://wger.de/identity/o/api/device/code\n    grant_types:\n      - authorization_code\n      - client_credentials\n   \
  \   - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:device_code'\n    docs: https://wger.readthedocs.io/en/latest/administration/oauth2_provider.html\n    sources:\n      - openapi/wger-openapi.yml\n      - https://wger.de/.well-known/openid-configuration\n  - name: cookieAuth\n    type: apiKey\n    in: cookie\n    parameter: sessionid\n    description: >-\n      The Django session cookie a logged-in browser already carries. Used by\n      wger's own web UI and by the browsable API.\n    sources:\n      - openapi/wger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wger/refs/heads/main/authentication/wger-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Sports And Fitness
- Public APIs
- Fitness
- Nutrition
- Health
- Open Source
- Self Hosted
- Workout Tracking
- Django
- REST
---
