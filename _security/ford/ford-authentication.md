---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ford-charging-api-openapi.yml
  format: yaml
  label: Ford Charging API
  slug: ford-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-charging-api-openapi.yml
- filename: ford-commands-api-openapi.yml
  format: yaml
  label: Ford Commands API
  slug: ford-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-commands-api-openapi.yml
- filename: ford-images-api-openapi.yml
  format: yaml
  label: Ford Images API
  slug: ford-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-images-api-openapi.yml
- filename: ford-oauth-api-openapi.yml
  format: yaml
  label: Ford OAuth API
  slug: ford-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-oauth-api-openapi.yml
- filename: ford-status-api-openapi.yml
  format: yaml
  label: Ford Status API
  slug: ford-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-status-api-openapi.yml
- filename: ford-vehicles-api-openapi.yml
  format: yaml
  label: Ford Vehicles API
  slug: ford-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-vehicles-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Ford Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ford secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ford
provider_slug: ford
scheme_count: 3
schemes:
- description: OAuth 2.0 authorization-code grant brokered through Ford Azure AD B2C; the user consents at https://fordconnect.cv.ford.com/common/login and the app receives a code it exchanges for a bearer token.
  flows:
  - authorizationUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/authorize
    claims_supported:
    - sub
    - idp
    - mtmId
    - userGuid
    - locale
    - jti
    - client_id
    - scope
    - iss
    - iat
    - exp
    - aud
    - acr
    - nonce
    - auth_time
    endSessionUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/logout
    flow: authorizationCode
    id_token_signing_alg_values_supported:
    - RS256
    issuer: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/v2.0/
    jwks_uri: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/discovery/v2.0/keys
    policy: B2C_1A_signup_signin_common
    response_modes_supported:
    - query
    - fragment
    - form_post
    response_types_supported:
    - code
    - code id_token
    - code token
    - code id_token token
    - id_token
    - id_token token
    - token
    - token id_token
    scopes_supported:
    - openid
    subject_types_supported:
    - pairwise
    tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/token
    token_endpoint_auth_methods_supported:
    - client_secret_post
    - client_secret_basic
  name: oauth2
  sources:
  - well-known/ford-openid-configuration.json
  type: oauth2
- bearerFormat: JWT
  description: 'The access token from the B2C token endpoint is sent as an Authorization: Bearer header on FordConnect API calls.'
  evidence: https://api.vehicle.ford.com/api/fordconnect/vehicleinfo/v3/vehicles returned HTTP 401 to an unauthenticated GET on 2026-09-10, confirming a live bearer-gated surface.
  name: bearerAuth
  scheme: bearer
  sources:
  - probe
  type: http
- confidence: medium
  description: FordConnect additionally requires the partner application id issued in the developer account dashboard alongside the bearer token.
  in: header
  name: applicationId
  note: Recorded from the credential surface Ford describes in the developer dashboard (Client ID / Secret 1 / Secret 2 / Expiration). The exact header name is not restated in any anonymously reachable Ford page — treat as medium confidence until an authenticated docs read confirms it.
  sources:
  - https://developer.ford.com/assets/i18n/en.json
  type: apiKey
  x-header: Application-Id
slug: ford-authentication
source_filename: ford-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/B2C_1A_signup_signin_common/v2.0/.well-known/openid-configuration\ndocs: https://developer.ford.com/apis\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  oauth2_flows:\n  - authorizationCode\n  primary: OAuth 2.0 authorization code against Ford's own Azure AD B2C consumer tenant, with vehicle-owner\n    consent captured as data categories\nnote: Upgraded from derived to searched on 2026-09-10 against Ford's own OpenID Connect discovery document,\n  fetched anonymously. The B2C tenant (dah2vb2cprod, 914d88b1-3523-4bf6-9be4-1b96b4f6f919) is Ford's —\n  it is the exact token endpoint Ford's FordConnect OAuth configuration names, and the same host the fordconnect.cv.ford.com\n  account-linking bundle calls. Credentials (client id + two rotating secrets) are issued from the signed-in\n  Ford Developer Marketplace account dashboard, not self-service\
  \ at runtime.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    issuer: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/v2.0/\n    authorizationUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/authorize\n    tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/token\n    endSessionUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/logout\n    jwks_uri: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/discovery/v2.0/keys\n    policy: B2C_1A_signup_signin_common\n    scopes_supported:\n    - openid\n    response_types_supported:\n    - code\n    - code id_token\n    - code token\n    - code id_token token\n    - id_token\n    - id_token token\n    - token\n    - token id_token\n    response_modes_supported:\n\
  \    - query\n    - fragment\n    - form_post\n    token_endpoint_auth_methods_supported:\n    - client_secret_post\n    - client_secret_basic\n    id_token_signing_alg_values_supported:\n    - RS256\n    subject_types_supported:\n    - pairwise\n    claims_supported:\n    - sub\n    - idp\n    - mtmId\n    - userGuid\n    - locale\n    - jti\n    - client_id\n    - scope\n    - iss\n    - iat\n    - exp\n    - aud\n    - acr\n    - nonce\n    - auth_time\n  description: OAuth 2.0 authorization-code grant brokered through Ford Azure AD B2C; the user consents\n    at https://fordconnect.cv.ford.com/common/login and the app receives a code it exchanges for a bearer\n    token.\n  sources:\n  - well-known/ford-openid-configuration.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'The access token from the B2C token endpoint is sent as an Authorization: Bearer header\n    on FordConnect API calls.'\n  evidence: https://api.vehicle.ford.com/api/fordconnect/vehicleinfo/v3/vehicles\
  \ returned HTTP 401 to\n    an unauthenticated GET on 2026-09-10, confirming a live bearer-gated surface.\n  sources:\n  - probe\n- name: applicationId\n  type: apiKey\n  in: header\n  x-header: Application-Id\n  description: FordConnect additionally requires the partner application id issued in the developer account\n    dashboard alongside the bearer token.\n  confidence: medium\n  note: Recorded from the credential surface Ford describes in the developer dashboard (Client ID / Secret\n    1 / Secret 2 / Expiration). The exact header name is not restated in any anonymously reachable Ford\n    page — treat as medium confidence until an authenticated docs read confirms it.\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\ncredentials:\n  issued_from: https://developer.ford.com/my-developer-account/my-profile\n  model: partner application registration; client id plus two rotatable secrets with an expiration date\n  self_serve: false\n  secret_rotation: two concurrent secrets\
  \ supported (\"Add Second Secret\"), each with its own expiration\n  redirect_uris: 1 required, maximum 5; https:// required except http:// for localhost\n  source: https://developer.ford.com/assets/i18n/en.json\nconsent:\n  model: vehicle-owner consent per data category, captured in the FordPass/Lincoln Way account-linking\n    flow\n  url: https://fordconnect.cv.ford.com/common/login\n  http_status: 200\n  categories: see scopes/ford-scopes.yml (14 data categories)\nx-evidence:\n- url: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/B2C_1A_signup_signin_common/v2.0/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-09-10'\n- url: https://fordconnect.cv.ford.com/common/login\n  http_status: 200\n  fetched: '2026-09-10'\n- url: https://api.vehicle.ford.com/api/fordconnect/vehicleinfo/v3/vehicles\n  http_status: 401\n  fetched: '2026-09-10'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/authentication/ford-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Automobiles
- Cars
- Vehicles
- Connected Vehicle
- Automotive
- Telematics
- Electric Vehicles
- Fleet
---
