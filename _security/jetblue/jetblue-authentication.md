---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jetblue Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
- deviceCode
- ciba
- refreshToken
overview: JetBlue secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, clientCredentials, deviceCode, ciba, and refreshToken flow(s).
provider_name: JetBlue
provider_slug: jetblue
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://accounts.jetblue.com/oauth2/v1/authorize
    device_authorization: https://accounts.jetblue.com/oauth2/v1/device/authorize
    end_session: https://accounts.jetblue.com/oauth2/v1/logout
    introspection: https://accounts.jetblue.com/oauth2/v1/introspect
    jwks: https://accounts.jetblue.com/oauth2/v1/keys
    pushed_authorization_request: https://accounts.jetblue.com/oauth2/v1/par
    registration: https://accounts.jetblue.com/oauth2/v1/clients
    revocation: https://accounts.jetblue.com/oauth2/v1/revoke
    token: https://accounts.jetblue.com/oauth2/v1/token
    userinfo: https://accounts.jetblue.com/oauth2/v1/userinfo
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:okta:params:oauth:grant-type:otp
  - urn:okta:params:oauth:grant-type:oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  id_token_encryption_alg_values_supported:
  - RSA-OAEP-256
  - RSA-OAEP-384
  - RSA-OAEP-512
  id_token_encryption_enc_values_supported:
  - A256GCM
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://accounts.jetblue.com
  name: JetBlueAccountsOIDC
  openIdConnectUrl: https://accounts.jetblue.com/.well-known/openid-configuration
  request_parameter_supported: true
  response_modes_supported:
  - query
  - fragment
  - form_post
  - okta_post_message
  response_types_supported:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  sources:
  - well-known/jetblue-openid-configuration.json
  - well-known/jetblue-oauth-authorization-server.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  vendor: Okta
slug: jetblue-authentication
source_filename: jetblue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://accounts.jetblue.com/.well-known/openid-configuration\nalso_source: https://accounts.jetblue.com/.well-known/oauth-authorization-server\ndocs: null\nscope_note: >-\n  JetBlue publishes no developer-facing authentication documentation. This\n  profile is read verbatim from the anonymous OpenID Connect / RFC 8414\n  discovery documents served by accounts.jetblue.com, the Okta-hosted identity\n  provider behind jetblue.com sign-in and the TrueBlue loyalty account. It\n  describes the CONSUMER identity surface used by JetBlue's own web and mobile\n  clients. It is not an authentication contract for third-party developers:\n  there is no published client-registration path for outside parties, and the\n  distribution (NDC / GDS) channel is gated behind ARC or IATA accreditation\n  plus JetBlue certification, with its auth model unpublished.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n\
  \  - implicit\n  - password\n  - clientCredentials\n  - deviceCode\n  - ciba\n  - refreshToken\n  api_key_in: []\n  pkce: true\n  pkce_methods:\n  - S256\n  dpop: true\n  par: true\n  mtls: false\nschemes:\n- name: JetBlueAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://accounts.jetblue.com/.well-known/openid-configuration\n  issuer: https://accounts.jetblue.com\n  vendor: Okta\n  endpoints:\n    authorization: https://accounts.jetblue.com/oauth2/v1/authorize\n    token: https://accounts.jetblue.com/oauth2/v1/token\n    userinfo: https://accounts.jetblue.com/oauth2/v1/userinfo\n    jwks: https://accounts.jetblue.com/oauth2/v1/keys\n    registration: https://accounts.jetblue.com/oauth2/v1/clients\n    introspection: https://accounts.jetblue.com/oauth2/v1/introspect\n    revocation: https://accounts.jetblue.com/oauth2/v1/revoke\n    end_session: https://accounts.jetblue.com/oauth2/v1/logout\n    device_authorization: https://accounts.jetblue.com/oauth2/v1/device/authorize\n\
  \    pushed_authorization_request: https://accounts.jetblue.com/oauth2/v1/par\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  - urn:okta:params:oauth:grant-type:otp\n  - urn:okta:params:oauth:grant-type:oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  response_types_supported:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  response_modes_supported:\n  - query\n  - fragment\n  - form_post\n  - okta_post_message\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - RS256\n  id_token_encryption_alg_values_supported:\n  - RSA-OAEP-256\n  - RSA-OAEP-384\n  - RSA-OAEP-512\n  id_token_encryption_enc_values_supported:\n\
  \  - A256GCM\n  code_challenge_methods_supported:\n  - S256\n  dpop_signing_alg_values_supported:\n  - RS256\n  - RS384\n  - RS512\n  - ES256\n  - ES384\n  - ES512\n  subject_types_supported:\n  - public\n  request_parameter_supported: true\n  sources:\n  - well-known/jetblue-openid-configuration.json\n  - well-known/jetblue-oauth-authorization-server.json\nundocumented_surfaces:\n- surface: NDC (IATA XML) partner API\n  auth_model: not-published\n  note: >-\n    JetBlue states it supplies NDC API documentation and message schemas only\n    to partners that pass business-use-case submission, onboarding and\n    certification testing (https://www.jetblue.com/travel-agents/ndc). No auth\n    model, endpoint or credential type is published.\n- surface: GDS / EDIFACT distribution\n  auth_model: out-of-band\n  note: >-\n    Access is an ARC (U.S.) or IATA + local BSP (international) accreditation\n    plus a JetBlue-granted, revocable ticketing authority; the technical\n    contract belongs\
  \ to the GDS, not JetBlue.\n- surface: api.jetblue.com\n  auth_model: not-published\n  note: Internal Fastly-fronted edge host for jetblue.com clients; 404 at every probed path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetblue/refs/heads/main/authentication/jetblue-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Travel
- United States
- Aviation
- Airline
- Distribution
- NDC
- GDS
- Booking
- Loyalty
---
