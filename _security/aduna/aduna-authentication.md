---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aduna Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- urn:ietf:params:oauth:grant-type:jwt-bearer
- ciba
overview: Aduna secures its APIs with oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, urn:ietf:params:oauth:grant-type:jwt-bearer, and ciba flow(s).
provider_name: Aduna
provider_slug: aduna
scheme_count: 4
schemes:
- acquisition_mode: AUTHORIZATION_CODE
  description: The device follows an Aduna-supplied invocation URL; the request results in a series of HTTP 302 responses until a final 200 carrying the verification result. State and a pre-registered redirect URL are required; when they are omitted no network-based option is returned by /auth/auth-info.
  flow: authorizationCode
  name: network-based authorization
  source: https://github.com/adunaglobal/nv2-asp-server-java-aduna-sdk#sdk-number-verification-overview
  type: oauth2
- acquisition_mode: JWT_BEARER_TOKEN
  description: RFC 7523 JWT-Bearer assertion flow. The ASP backend signs assertions with keys it manages and publishes; Aduna fetches the public keys from a single ASP-hosted JWKS URL supplied at onboarding. The SDK rotates signing keys on a configurable interval (default P90D, requested key TTL P91D) via the JwtBearerTokenKeyManager / JwtBearerTokenKeyRotator interfaces.
  flow: urn:ietf:params:oauth:grant-type:jwt-bearer
  integrator_requirements:
  - /.well-known/openid-configuration on the ASP backend exposing issuer, jwks_uri and subject_types_supported
  - /jwks on the ASP backend returning every public key used to sign assertions, across all instances
  name: SIM-based authorization (JWT-Bearer)
  recommended: true
  type: oauth2
- acquisition_mode: CIBA
  description: OpenID Connect Client-Initiated Backchannel Authentication. POST /auth/bc-authorize returns a CibaResponse carrying auth_req_id, expires_in and a polling interval; the token is then collected from POST /auth/token.
  flow: ciba
  name: SIM-based authorization (CIBA)
  type: oauth2
- description: 'All CAMARA resource calls carry Authorization: Bearer <access token> obtained from POST /auth/token. Tokens are returned with type and expires_in.'
  name: bearer access token
  scheme: bearer
  type: http
slug: aduna-authentication
source_filename: aduna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://github.com/adunaglobal/nv2-asp-server-java-aduna-sdk\ndocs: https://docs.adunaglobal.com/how-to-enable-an-api/number-verification-api-v-2.1-landing-page\ndocs_gated: true\nnote: >-\n  Aduna publishes no OpenAPI, so this profile is read verbatim from Aduna's own source-available\n  Java SDK (Feign clients, configuration classes and README) rather than derived from a spec. The\n  reference documentation exists but every path on docs.adunaglobal.com redirects to an Auth0 login\n  wall, so the authoritative public evidence is the SDK source.\nsummary:\n  types: [oauth2, openIdConnect, http]\n  oauth2_flows: [authorizationCode, urn:ietf:params:oauth:grant-type:jwt-bearer, ciba]\n  api_key_in: []\n  bearer_token: true\n  mutual_tls: false\n  self_service: false\n  onboarding: >-\n    Client ID and client secret are issued per ASP application during a manual onboarding\n    conversation. The SDK README states: \"Contact Aduna\
  \ Global for the onboarding procedure of an\n    ASP Application.\" Redirect URLs must be registered with Aduna at onboarding and are validated\n    by the Aduna platform on every authorization-code request.\nschemes:\n- name: network-based authorization\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    The device follows an Aduna-supplied invocation URL; the request results in a series of HTTP 302\n    responses until a final 200 carrying the verification result. State and a pre-registered\n    redirect URL are required; when they are omitted no network-based option is returned by\n    /auth/auth-info.\n  acquisition_mode: AUTHORIZATION_CODE\n  source: https://github.com/adunaglobal/nv2-asp-server-java-aduna-sdk#sdk-number-verification-overview\n- name: SIM-based authorization (JWT-Bearer)\n  type: oauth2\n  flow: urn:ietf:params:oauth:grant-type:jwt-bearer\n  recommended: true\n  description: >-\n    RFC 7523 JWT-Bearer assertion flow. The ASP backend signs assertions\
  \ with keys it manages and\n    publishes; Aduna fetches the public keys from a single ASP-hosted JWKS URL supplied at\n    onboarding. The SDK rotates signing keys on a configurable interval (default P90D, requested\n    key TTL P91D) via the JwtBearerTokenKeyManager / JwtBearerTokenKeyRotator interfaces.\n  acquisition_mode: JWT_BEARER_TOKEN\n  integrator_requirements:\n  - /.well-known/openid-configuration on the ASP backend exposing issuer, jwks_uri and subject_types_supported\n  - /jwks on the ASP backend returning every public key used to sign assertions, across all instances\n- name: SIM-based authorization (CIBA)\n  type: oauth2\n  flow: ciba\n  description: >-\n    OpenID Connect Client-Initiated Backchannel Authentication. POST /auth/bc-authorize returns a\n    CibaResponse carrying auth_req_id, expires_in and a polling interval; the token is then\n    collected from POST /auth/token.\n  acquisition_mode: CIBA\n- name: bearer access token\n  type: http\n  scheme: bearer\n  description:\
  \ >-\n    All CAMARA resource calls carry Authorization: Bearer <access token> obtained from\n    POST /auth/token. Tokens are returned with type and expires_in.\nendpoints:\n- method: POST\n  path: /auth/auth-info\n  purpose: >-\n    Discover the authorization options available for a phone number or PLMN ID. Returns\n    networkBasedAuthZData (an invocation URL) and/or simBasedAuthZData (iOS App Clip URL, Android\n    app URL, app-info JWT and callback query parameter names).\n  request_fields: [phoneNumber, plmnId, scopes, appId, appName, appCallbackUrl, nonce, vpRequest, state, redirectUrl]\n  query_parameters: [lang]\n- method: POST\n  path: /auth/bc-authorize\n  purpose: CIBA backchannel authentication request.\n  content_type: application/x-www-form-urlencoded\n- method: POST\n  path: /auth/token\n  purpose: Token endpoint for the authorization-code, JWT-Bearer and CIBA flows.\n  content_type: application/x-www-form-urlencoded\nbase_url:\n  published: false\n  note: >-\n    Both\
  \ Feign clients bind to the injected configuration property\n    ${com.adunaglobal.sdk.backend.connection.baseURL}. The host is supplied to a partner at\n    onboarding; Aduna publishes no production base URL, so none is asserted here.\nheaders:\n- name: Authorization\n  required: true\n  note: Client credentials on the /auth endpoints; Bearer access token on the CAMARA endpoints.\n- name: X-Correlator\n  required: true\n  note: Random UUID generated per request by the SDK; carried on both auth and resource calls.\naduna_authorization_api_version: v1.4.0\nportal_identity_provider:\n  issuer: https://prod-aduna-global.us.auth0.com/\n  well_known: https://prod-aduna-global.us.auth0.com/.well-known/openid-configuration\n  status: 200\n  artifact: well-known/aduna-portal-auth0-openid-configuration.json\n  note: >-\n    Auth0 tenant guarding the Aduna developer portal and documentation — NOT the network-API\n    authorization server. Advertises authorization_code, device_authorization, userinfo,\
  \ revocation\n    and dynamic client registration, S256 PKCE, and client_secret_basic / client_secret_post /\n    private_key_jwt / none client authentication. Its scopes_supported are stock Auth0 OIDC profile\n    claims, not CAMARA scopes.\nrelated:\n  scopes: scopes/aduna-scopes.yml\n  conventions: conventions/aduna-conventions.yml\n  errors: errors/aduna-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aduna/refs/heads/main/authentication/aduna-authentication.yml
summary_line: oauth2/openIdConnect/http · 4 schemes
tags:
- Telecommunications
- Sweden
- Network APIs
- CAMARA
- Open Gateway
- API Aggregator
- Identity Verification
- SIM Swap
- Number Verification
- Fraud Prevention
- Quality on Demand
- Device Location
- Ericsson
---
