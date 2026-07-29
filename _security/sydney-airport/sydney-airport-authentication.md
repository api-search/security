---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sydney Airport Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- deviceCode
- ciba
- jwtBearer
- saml2Bearer
- umaTicket
- refreshToken
overview: Sydney Airport secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, deviceCode, ciba, jwtBearer, saml2Bearer, umaTicket, and refreshToken flow(s).
provider_name: Sydney Airport
provider_slug: sydney-airport
scheme_count: 2
schemes:
- acr_values:
  - SYDLogin
  issuer: https://id.syd.com.au:443/am/oauth2
  name: SYDLogin
  openIdConnectUrl: https://id.syd.com.au/am/oauth2/.well-known/openid-configuration
  sources:
  - authentication/sydney-airport-openid-configuration.json
  type: openIdConnect
  vendor: ForgeRock Access Management (realm /alpha)
  version: '3.0'
- flows:
  - authorizationUrl: https://id.syd.com.au:443/am/oauth2/authorize
    flow: authorizationCode
    observed_client: INFOSYD_APP_Client
    observed_redirect_uri: https://sydneyairport.com.au/infosyd/callback
    observed_scope: openid profile email infosyd
    pkce: true
    pkce_methods:
    - S256
    - plain
    refreshUrl: https://id.syd.com.au:443/am/oauth2/access_token
    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token
  - authorizationUrl: https://id.syd.com.au:443/am/oauth2/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token
  - flow: password
    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token
  name: SYDOAuth2
  sources:
  - authentication/sydney-airport-openid-configuration.json
  type: oauth2
slug: sydney-airport-authentication
source_filename: sydney-airport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: authentication/sydney-airport-openid-configuration.json\ndocs: null\nnote: >-\n  Sydney Airport publishes no public API and therefore no OpenAPI securitySchemes.\n  The only machine-readable authentication contract it publishes is the OpenID\n  Connect Discovery 1.0 document for the ForgeRock Access Management realm that\n  fronts InfoSYD, its gated airline / ground-handler / on-airport-tenant portal.\n  Everything below is derived verbatim from that document (harvested 2026-07-28,\n  HTTP 200) plus the authorize request observed on the InfoSYD login redirect.\n  It describes how a credentialed partner authenticates - it does not describe any\n  callable resource API, because none is published.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - password\n  - deviceCode\n  - ciba\n  - jwtBearer\n  - saml2Bearer\n  - umaTicket\n\
  \  - refreshToken\n  public_self_serve: false\n  audience: airlines, ground handlers, border agencies and on-airport tenants with a\n    commercial or operational relationship with Sydney Airport Corporation Limited\nschemes:\n- name: SYDLogin\n  type: openIdConnect\n  openIdConnectUrl: https://id.syd.com.au/am/oauth2/.well-known/openid-configuration\n  issuer: https://id.syd.com.au:443/am/oauth2\n  vendor: ForgeRock Access Management (realm /alpha)\n  version: '3.0'\n  acr_values: [SYDLogin]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n- name: SYDOAuth2\n  type: oauth2\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.syd.com.au:443/am/oauth2/authorize\n    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token\n    refreshUrl: https://id.syd.com.au:443/am/oauth2/access_token\n    pkce: true\n    pkce_methods: [S256, plain]\n    observed_client: INFOSYD_APP_Client\n\
  \    observed_scope: openid profile email infosyd\n    observed_redirect_uri: https://sydneyairport.com.au/infosyd/callback\n  - flow: implicit\n    authorizationUrl: https://id.syd.com.au:443/am/oauth2/authorize\n  - flow: clientCredentials\n    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token\n  - flow: password\n    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token\nendpoints:\n  authorization: https://id.syd.com.au:443/am/oauth2/authorize\n  token: https://id.syd.com.au:443/am/oauth2/access_token\n  userinfo: https://id.syd.com.au:443/am/oauth2/userinfo\n  jwks: https://id.syd.com.au:443/am/oauth2/connect/jwk_uri\n  introspection: https://id.syd.com.au:443/am/oauth2/introspect\n  revocation: https://id.syd.com.au:443/am/oauth2/token/revoke\n  registration: https://id.syd.com.au:443/am/oauth2/register\n  pushed_authorization_request: https://id.syd.com.au:443/am/oauth2/par\n  end_session: https://id.syd.com.au:443/am/oauth2/connect/endSession\n  check_session_iframe:\
  \ https://id.syd.com.au:443/am/oauth2/connect/checkSession\nclient_authentication:\n  methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\n  - none\n  mtls_bound_access_tokens: true\n  require_pushed_authorization_requests: false\n  require_request_uri_registration: true\ntokens:\n  id_token_signing_alg: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512,\n    HS256, HS384, HS512]\n  id_token_encryption_alg: [RSA-OAEP, RSA-OAEP-256, ECDH-ES, ECDH-ES+A128KW, ECDH-ES+A192KW,\n    ECDH-ES+A256KW, A128KW, A192KW, A256KW, dir]\n  subject_types: [public, pairwise]\n  response_types: [code, 'code id_token', 'code token', 'code token id_token', id_token,\n    token, 'token id_token', device_code]\n  response_modes: [query, fragment, form_post, jwt, query.jwt, fragment.jwt, form_post.jwt]\n  backchannel_logout_supported: true\nunauthenticated_surfaces:\n- url: https://www.sydneyairport.com.au/_a/flights\n\
  \  auth: none\n  note: Undocumented website backend. No key, no token, no published contract; the\n    site terms of use prohibit automated retrieval.\n- url: https://www.sydneyairport.com.au/_a/security-wait-times\n  auth: none\n  note: Undocumented website backend, same posture.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sydney-airport/refs/heads/main/authentication/sydney-airport-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Travel
- Australia
- Airports
- Aviation
- Airport Infrastructure
- Transportation
- Flight Information
- Passenger Experience
---
