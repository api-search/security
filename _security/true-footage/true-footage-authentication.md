---
api_key_in: []
auth_types: []
description: True Footage publishes no developer documentation and no OpenAPI, so this profile is built entirely from the two OpenID Connect discovery documents its identity hosts serve anonymously, plus the observed behaviour of the two product API hosts. Both product surfaces (TrueTracts and TrueEngine) sit behind an Auth0 custom identity domain; the product APIs themselves reject every unauthenticated request at the edge.
kind: authentication
layout: security
method: probed
name: True Footage Authentication
name_suffix: Authentication
oauth_flows: []
overview: True Footage declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: True Footage
provider_slug: true-footage
scheme_count: 2
schemes:
- applies_to: TrueTracts appraiser console (truetracts.truefootage.tech) and api.truetracts.truefootage.tech
  endpoints:
    authorization: https://auth.truetracts.truefootage.tech/authorize
    device_authorization: https://auth.truetracts.truefootage.tech/oauth/device/code
    jwks: https://auth.truetracts.truefootage.tech/.well-known/jwks.json
    mfa_challenge: https://auth.truetracts.truefootage.tech/mfa/challenge
    registration: https://auth.truetracts.truefootage.tech/oidc/register
    revocation: https://auth.truetracts.truefootage.tech/oauth/revoke
    token: https://auth.truetracts.truefootage.tech/oauth/token
    userinfo: https://auth.truetracts.truefootage.tech/userinfo
  issuer: https://auth.truetracts.truefootage.tech/
  key: truetracts_oidc
  openIdConnectUrl: https://auth.truetracts.truefootage.tech/.well-known/openid-configuration
  type: openIdConnect
  x-evidence:
    content_type: application/json
    fetched: '2026-08-05'
    file: well-known/true-footage-truetracts-openid-configuration.json
    http_status: 200
    url: https://auth.truetracts.truefootage.tech/.well-known/openid-configuration
- applies_to: TrueEngine (trueengine.truefootage.tech) and api.trueengine.truefootage.tech
  endpoints:
    authorization: https://auth.trueengine.truefootage.tech/authorize
    jwks: https://auth.trueengine.truefootage.tech/.well-known/jwks.json
    token: https://auth.trueengine.truefootage.tech/oauth/token
    userinfo: https://auth.trueengine.truefootage.tech/userinfo
  issuer: https://auth.trueengine.truefootage.tech/
  key: trueengine_oidc
  openIdConnectUrl: https://auth.trueengine.truefootage.tech/.well-known/openid-configuration
  type: openIdConnect
  x-evidence:
    content_type: application/json
    fetched: '2026-08-05'
    file: well-known/true-footage-trueengine-openid-configuration.json
    http_status: 200
    url: https://auth.trueengine.truefootage.tech/.well-known/openid-configuration
slug: true-footage-authentication
source_filename: true-footage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://auth.truetracts.truefootage.tech/.well-known/openid-configuration\ndescription: >-\n  True Footage publishes no developer documentation and no OpenAPI, so this profile is\n  built entirely from the two OpenID Connect discovery documents its identity hosts serve\n  anonymously, plus the observed behaviour of the two product API hosts. Both product\n  surfaces (TrueTracts and TrueEngine) sit behind an Auth0 custom identity domain; the\n  product APIs themselves reject every unauthenticated request at the edge.\nsummary:\n  model: oauth2-oidc\n  provider: Auth0 (custom identity domains under truefootage.tech)\n  public_api_program: false\n  note: >-\n    These are the tenant-facing sign-in surfaces for True Footage's own SaaS products,\n    not a documented third-party API program. No client registration flow, scope\n    reference, or key-issuance page is published publicly.\nschemes:\n  - key: truetracts_oidc\n    type:\
  \ openIdConnect\n    openIdConnectUrl: https://auth.truetracts.truefootage.tech/.well-known/openid-configuration\n    issuer: https://auth.truetracts.truefootage.tech/\n    applies_to: TrueTracts appraiser console (truetracts.truefootage.tech) and api.truetracts.truefootage.tech\n    endpoints:\n      authorization: https://auth.truetracts.truefootage.tech/authorize\n      token: https://auth.truetracts.truefootage.tech/oauth/token\n      userinfo: https://auth.truetracts.truefootage.tech/userinfo\n      jwks: https://auth.truetracts.truefootage.tech/.well-known/jwks.json\n      revocation: https://auth.truetracts.truefootage.tech/oauth/revoke\n      registration: https://auth.truetracts.truefootage.tech/oidc/register\n      device_authorization: https://auth.truetracts.truefootage.tech/oauth/device/code\n      mfa_challenge: https://auth.truetracts.truefootage.tech/mfa/challenge\n    x-evidence:\n      fetched: '2026-08-05'\n      url: https://auth.truetracts.truefootage.tech/.well-known/openid-configuration\n\
  \      http_status: 200\n      content_type: application/json\n      file: well-known/true-footage-truetracts-openid-configuration.json\n  - key: trueengine_oidc\n    type: openIdConnect\n    openIdConnectUrl: https://auth.trueengine.truefootage.tech/.well-known/openid-configuration\n    issuer: https://auth.trueengine.truefootage.tech/\n    applies_to: TrueEngine (trueengine.truefootage.tech) and api.trueengine.truefootage.tech\n    endpoints:\n      authorization: https://auth.trueengine.truefootage.tech/authorize\n      token: https://auth.trueengine.truefootage.tech/oauth/token\n      userinfo: https://auth.trueengine.truefootage.tech/userinfo\n      jwks: https://auth.trueengine.truefootage.tech/.well-known/jwks.json\n    x-evidence:\n      fetched: '2026-08-05'\n      url: https://auth.trueengine.truefootage.tech/.well-known/openid-configuration\n      http_status: 200\n      content_type: application/json\n      file: well-known/true-footage-trueengine-openid-configuration.json\n\
  capabilities:\n  pkce:\n    supported: true\n    code_challenge_methods: [S256, plain]\n  grant_types:\n    - client_credentials\n    - authorization_code\n    - refresh_token\n    - password\n    - implicit\n    - 'urn:ietf:params:oauth:grant-type:device_code'\n    - 'urn:ietf:params:oauth:grant-type:token-exchange'\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods:\n    - client_secret_basic\n    - client_secret_post\n    - private_key_jwt\n    - none\n  id_token_signing_alg_values: [HS256, RS256, PS256]\n  mfa: true\n  note_scopes: >-\n    scopes_supported advertises only the fourteen standard OIDC identity scopes\n    (openid, profile, offline_access, email, phone, address and the individual claim\n    scopes). These are Auth0 tenant defaults, not a designed API permission surface —\n    no product-specific scopes are published, so no scopes/ artifact is emitted.\naccess:\n  status: gated\n  observed:\n    - url: https://api.truetracts.truefootage.tech/\n\
  \      http_status: 401\n      body: '{\"detail\":\"authorization header is expected\"}'\n    - url: https://api.truetracts.truefootage.tech/openapi.json\n      http_status: 401\n    - url: https://api.trueengine.truefootage.tech/openapi.json\n      http_status: 401\n    - url: https://api.truetracts.truefootage.tech/health\n      http_status: 200\n      body: '{}'\n  note: >-\n    Both product APIs reject unauthenticated requests uniformly, including the spec and\n    docs paths a FastAPI-shaped service would normally serve anonymously. Credentials are\n    issued through the product signup, not through a developer program.\ngaps:\n  - No public developer portal, API reference, or key-issuance page.\n  - No machine-readable contract (OpenAPI/GraphQL/AsyncAPI) reachable without a token.\n  - >-\n    No /.well-known/oauth-protected-resource on either API host, so an agent cannot\n    discover which authorization server protects which resource.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-footage/refs/heads/main/authentication/true-footage-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Real-Estate
- Appraisal
- Valuation
- PropTech
- Mortgage
- Property Data
- Analytics
- Machine-Learning
---
