---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: 'E.ON Next has exactly one publicly describable authentication surface, and it is customer sign-in, not developer access: an OpenID Connect / OAuth 2.0 authorization server at https://auth.eonnext.com/, run on Auth0 as the E.ON group CIAM tenant (certificate CN eon-next-uk.eon-ciam.auth0app.com, Cloudflare edge, Let''s Encrypt certificate). Its RFC 8414 / OIDC Discovery metadata is served anonymously and completely, so the grant types, endpoints, signing keys and client-authentication methods below are observed fact rather than inference. What the discovery document does NOT imply is a developer programme: there is no published client registration path for a third party, no API-key programme, no partner onboarding and no documented resource server. The application-facing hosts api.eonnext.com and data.eonnext.com sit behind AWS API Gateway and answer every anonymous request with {"message":"Missing Authentication Token"} (HTTP 403), disclosing no scheme at all. Treat this artifact
  as "how an E.ON Next customer''s browser or app authenticates", not "how you get an API credential".'
kind: authentication
layout: security
method: searched
name: Eon Next Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- deviceCode
- refreshToken
- tokenExchange
- ciba
overview: E.ON Next secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, deviceCode, refreshToken, tokenExchange, and ciba flow(s).
provider_name: E.ON Next
provider_slug: eon-next
scheme_count: 2
schemes:
- backchannel_logout_supported: true
  backchannel_token_delivery_modes_supported:
  - poll
  claims_supported:
  - aud
  - auth_time
  - created_at
  - email
  - email_verified
  - exp
  - family_name
  - given_name
  - iat
  - identities
  - iss
  - name
  - nickname
  - phone_number
  - picture
  - sub
  code_challenge_methods_supported:
  - S256
  - plain
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://auth.eonnext.com/authorize
    backchannel_authentication: https://auth.eonnext.com/bc-authorize
    device_authorization: https://auth.eonnext.com/oauth/device/code
    end_session: https://auth.eonnext.com/oidc/logout
    global_token_revocation: https://auth.eonnext.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.eonnext.com/.well-known/jwks.json
    mfa_challenge: https://auth.eonnext.com/mfa/challenge
    pushed_authorization_request: null
    registration: https://auth.eonnext.com/oidc/register
    revocation: https://auth.eonnext.com/oauth/revoke
    token: https://auth.eonnext.com/oauth/token
    userinfo: https://auth.eonnext.com/userinfo
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.eonnext.com/
  keys:
    algorithms:
    - RS256
    jwks_file: well-known/eon-next-jwks.json
    key_count: 2
  mfa: Multi-factor is a first-class part of this tenant — a dedicated /mfa/challenge endpoint plus mfa-oob, mfa-otp and mfa-recovery-code grants.
  name: eon-next-ciam-oidc
  openIdConnectUrl: https://auth.eonnext.com/.well-known/openid-configuration
  request_object_signing_alg_values_supported:
  - RS256
  - RS384
  - PS256
  request_parameter_supported: true
  request_uri_parameter_supported: false
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  scopes: see scopes/eon-next-scopes.yml
  sources:
  - well-known/eon-next-openid-configuration.json
  subject_types_supported:
  - public
  tls_client_certificate_bound_access_tokens: true
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  - none
  token_endpoint_auth_signing_alg_values_supported:
  - RS256
  - RS384
  - PS256
  type: openIdConnect
  vendor: Auth0 (Okta) — E.ON group CIAM tenant "eon-ciam", application "eon-next-uk"
- documented: false
  hosts:
  - https://api.eonnext.com
  - https://data.eonnext.com
  name: aws-api-gateway-undisclosed
  observed: HTTP 403 with the 42-byte body {"message":"Missing Authentication Token"} on every probed path, including /.well-known/*, /openapi.json, /graphql and /health. This is the canonical AWS API Gateway response for an unmatched or unauthorised route. It proves a gateway is deployed; it discloses neither the authorizer type nor any credential model.
  type: unknown
slug: eon-next-authentication
source_filename: eon-next-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://auth.eonnext.com/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  There is no human-readable authentication documentation. Everything below was\n  read out of the authorization server's own anonymous discovery document\n  (HTTP 200 on 2026-07-27), not out of a developer portal — E.ON Next publishes\n  none.\ndescription: >-\n  E.ON Next has exactly one publicly describable authentication surface, and it\n  is customer sign-in, not developer access: an OpenID Connect / OAuth 2.0\n  authorization server at https://auth.eonnext.com/, run on Auth0 as the E.ON\n  group CIAM tenant (certificate CN eon-next-uk.eon-ciam.auth0app.com, Cloudflare\n  edge, Let's Encrypt certificate). Its RFC 8414 / OIDC Discovery metadata is\n  served anonymously and completely, so the grant types, endpoints, signing keys\n  and client-authentication methods below are observed fact rather than\n  inference. What the discovery document\
  \ does NOT imply is a developer\n  programme: there is no published client registration path for a third party,\n  no API-key programme, no partner onboarding and no documented resource server.\n  The application-facing hosts api.eonnext.com and data.eonnext.com sit behind\n  AWS API Gateway and answer every anonymous request with\n  {\"message\":\"Missing Authentication Token\"} (HTTP 403), disclosing no scheme at\n  all. Treat this artifact as \"how an E.ON Next customer's browser or app\n  authenticates\", not \"how you get an API credential\".\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, password, deviceCode, refreshToken, tokenExchange, ciba]\n  third_party_access: none-published\nschemes:\n- name: eon-next-ciam-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.eonnext.com/.well-known/openid-configuration\n  issuer: https://auth.eonnext.com/\n  vendor: Auth0 (Okta) — E.ON group CIAM tenant\
  \ \"eon-ciam\", application \"eon-next-uk\"\n  sources: [well-known/eon-next-openid-configuration.json]\n  endpoints:\n    authorization: https://auth.eonnext.com/authorize\n    token: https://auth.eonnext.com/oauth/token\n    userinfo: https://auth.eonnext.com/userinfo\n    jwks: https://auth.eonnext.com/.well-known/jwks.json\n    registration: https://auth.eonnext.com/oidc/register\n    revocation: https://auth.eonnext.com/oauth/revoke\n    end_session: https://auth.eonnext.com/oidc/logout\n    device_authorization: https://auth.eonnext.com/oauth/device/code\n    backchannel_authentication: https://auth.eonnext.com/bc-authorize\n    mfa_challenge: https://auth.eonnext.com/mfa/challenge\n    global_token_revocation: https://auth.eonnext.com/oauth/global-token-revocation/connection/{connectionName}\n    pushed_authorization_request: null\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types_supported: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - tls_client_auth\n  - self_signed_tls_client_auth\n  - none\n  token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, PS256]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  request_object_signing_alg_values_supported: [RS256, RS384, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  tls_client_certificate_bound_access_tokens:\
  \ true\n  request_parameter_supported: true\n  request_uri_parameter_supported: false\n  backchannel_logout_supported: true\n  backchannel_token_delivery_modes_supported: [poll]\n  subject_types_supported: [public]\n  claims_supported: [aud, auth_time, created_at, email, email_verified, exp, family_name, given_name, iat, identities, iss, name, nickname, phone_number, picture, sub]\n  scopes: see scopes/eon-next-scopes.yml\n  mfa: >-\n    Multi-factor is a first-class part of this tenant — a dedicated\n    /mfa/challenge endpoint plus mfa-oob, mfa-otp and mfa-recovery-code grants.\n  keys:\n    jwks_file: well-known/eon-next-jwks.json\n    key_count: 2\n    algorithms: [RS256]\n- name: aws-api-gateway-undisclosed\n  type: unknown\n  hosts: [https://api.eonnext.com, https://data.eonnext.com]\n  observed: >-\n    HTTP 403 with the 42-byte body {\"message\":\"Missing Authentication Token\"} on\n    every probed path, including /.well-known/*, /openapi.json, /graphql and\n    /health. This\
  \ is the canonical AWS API Gateway response for an unmatched or\n    unauthorised route. It proves a gateway is deployed; it discloses neither the\n    authorizer type nor any credential model.\n  documented: false\nnotes:\n- >-\n  A registration_endpoint (/oidc/register) is advertised, which is OAuth 2.0\n  Dynamic Client Registration (RFC 7591). Auth0 advertises it whether or not the\n  tenant permits open registration; it was NOT exercised, so no claim is made\n  that a third party can self-register a client.\n- >-\n  No Pushed Authorization Request endpoint and no FAPI profile are advertised,\n  so this is a mainstream CIAM configuration rather than a regulated\n  open-banking/open-energy style deployment.\n- >-\n  Britain has no consumer energy data-portability mandate, so there is no\n  regulated accreditation model (nothing equivalent to Australian CDR ADR\n  accreditation or an FDX/OAuth data-sharing profile) sitting behind this server.\n  See review.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon-next/refs/heads/main/authentication/eon-next-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Retail
- Kraken
- Solar
- EV Charging
- Identity
---
