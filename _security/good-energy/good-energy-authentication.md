---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Good Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- deviceCode
- ciba
overview: Good Energy secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, deviceCode, and ciba flow(s).
provider_name: Good Energy
provider_slug: good-energy
scheme_count: 1
schemes:
- dpop:
    signing_algs:
    - RS256
    - RS384
    - RS512
    - PS256
    - PS384
    - PS512
    - ES256
    - ES384
    - ES512
  dynamic_client_registration: false
  endpoints:
    authorization: https://login.goodenergy.co.uk/connect/authorize
    backchannel_authentication: https://login.goodenergy.co.uk/connect/ciba
    check_session_iframe: https://login.goodenergy.co.uk/connect/checksession
    device_authorization: https://login.goodenergy.co.uk/connect/deviceauthorization
    end_session: https://login.goodenergy.co.uk/connect/endsession
    introspection: https://login.goodenergy.co.uk/connect/introspect
    jwks: https://login.goodenergy.co.uk/.well-known/openid-configuration/jwks
    pushed_authorization_request: https://login.goodenergy.co.uk/connect/par
    registration: null
    revocation: https://login.goodenergy.co.uk/connect/revocation
    token: https://login.goodenergy.co.uk/connect/token
    userinfo: https://login.goodenergy.co.uk/connect/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_signing_algs:
  - RS256
  issuer: https://login.goodenergy.co.uk
  logout:
    backchannel: true
    backchannel_session: true
    frontchannel: true
    frontchannel_session: true
  mutual_tls: false
  name: GoodEnergyCustomerIdentity
  openIdConnectUrl: https://login.goodenergy.co.uk/.well-known/openid-configuration
  par:
    required: false
    supported: true
  pkce:
    methods:
    - plain
    - S256
    supported: true
  prompt_values:
  - none
  - login
  - consent
  - select_account
  - create
  request_object_signing_algs:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  response_modes:
  - form_post
  - query
  - fragment
  response_types:
  - code
  - token
  - id_token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - customer_portal
  - customer_portal_tariff_switch
  sources:
  - authentication/good-energy-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  vendor_shape: Duende IdentityServer
slug: good-energy-authentication
source_filename: good-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: authentication/good-energy-openid-configuration.json\nsource_url: https://login.goodenergy.co.uk/.well-known/openid-configuration\nfetched: '2026-07-27'\nhttp_status: 200\nnote: >-\n  Derived verbatim from the live OpenID Connect Discovery document of Good Energy's customer-login\n  identity provider. There is no OpenAPI to derive securitySchemes from — Good Energy publishes no\n  developer-facing API — so this profile describes the ONLY authenticated surface the company exposes\n  anonymously in machine-readable form. It is a customer portal login, not a developer API auth\n  model: there is no registration_endpoint, so dynamic client registration is unavailable and no\n  third party can obtain a client. Access is customer-account-required.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - password\n  - deviceCode\n  - ciba\n\
  \  developer_accessible: false\n  gate: customer-account-required\nschemes:\n- name: GoodEnergyCustomerIdentity\n  type: openIdConnect\n  openIdConnectUrl: https://login.goodenergy.co.uk/.well-known/openid-configuration\n  issuer: https://login.goodenergy.co.uk\n  vendor_shape: Duende IdentityServer\n  sources:\n  - authentication/good-energy-openid-configuration.json\n  endpoints:\n    authorization: https://login.goodenergy.co.uk/connect/authorize\n    token: https://login.goodenergy.co.uk/connect/token\n    userinfo: https://login.goodenergy.co.uk/connect/userinfo\n    jwks: https://login.goodenergy.co.uk/.well-known/openid-configuration/jwks\n    introspection: https://login.goodenergy.co.uk/connect/introspect\n    revocation: https://login.goodenergy.co.uk/connect/revocation\n    end_session: https://login.goodenergy.co.uk/connect/endsession\n    check_session_iframe: https://login.goodenergy.co.uk/connect/checksession\n    device_authorization: https://login.goodenergy.co.uk/connect/deviceauthorization\n\
  \    backchannel_authentication: https://login.goodenergy.co.uk/connect/ciba\n    pushed_authorization_request: https://login.goodenergy.co.uk/connect/par\n    registration: null\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  response_types:\n  - code\n  - token\n  - id_token\n  - id_token token\n  - code id_token\n  - code token\n  - code id_token token\n  response_modes:\n  - form_post\n  - query\n  - fragment\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  pkce:\n    supported: true\n    methods:\n    - plain\n    - S256\n  par:\n    supported: true\n    required: false\n  dpop:\n    signing_algs:\n    - RS256\n    - RS384\n    - RS512\n    - PS256\n    - PS384\n    - PS512\n    - ES256\n    - ES384\n    - ES512\n  id_token_signing_algs:\n  - RS256\n  subject_types:\n  - public\n  request_object_signing_algs:\n\
  \  - RS256\n  - RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\n  - HS256\n  - HS384\n  - HS512\n  logout:\n    frontchannel: true\n    frontchannel_session: true\n    backchannel: true\n    backchannel_session: true\n  prompt_values:\n  - none\n  - login\n  - consent\n  - select_account\n  - create\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - customer_portal\n  - customer_portal_tariff_switch\n  mutual_tls: false\n  dynamic_client_registration: false\nobservations:\n- >-\n  Legacy grants are still advertised alongside modern ones — implicit and resource-owner password\n  remain in grant_types_supported, and plain is still an accepted PKCE code_challenge_method.\n- No mTLS / private_key_jwt client authentication is advertised; only client_secret_basic and\n  client_secret_post.\n- No registration_endpoint, so there is no self-serve or dynamic path to a client_id for a third\n  party — the surface is closed to developers by\
  \ construction, not by policy statement.\ncross_references:\n  scopes: scopes/good-energy-scopes.yml\n  well_known: well-known/good-energy-well-known.yml\n  conformance: conformance/good-energy-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-energy/refs/heads/main/authentication/good-energy-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Renewables
- Smart Metering
- Solar
- EV Charging
- Energy Retail
---
