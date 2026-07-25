---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Nib Health Funds Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
- tokenExchange
- jwtBearer
overview: nib secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, deviceCode, tokenExchange, and jwtBearer flow(s).
provider_name: nib
provider_slug: nib-health-funds
scheme_count: 3
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
  discovery_status: 200
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://id.nib.com.au/authorize
    backchannel_authentication: https://id.nib.com.au/bc-authorize
    device_authorization: https://id.nib.com.au/oauth/device/code
    global_token_revocation: https://id.nib.com.au/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://id.nib.com.au/.well-known/jwks.json
    mfa_challenge: https://id.nib.com.au/mfa/challenge
    registration: https://id.nib.com.au/oidc/register
    revocation: https://id.nib.com.au/oauth/revoke
    token: https://id.nib.com.au/oauth/token
    userinfo: https://id.nib.com.au/userinfo
  grant_types_supported:
  - client_credentials
  - authorization_code
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
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://id.nib.com.au/
  jwks:
    algs:
    - RS256
    file: well-known/nib-health-funds-jwks.json
    keys: 2
  name: nib Australia member identity (Auth0 OIDC)
  openIdConnectUrl: https://id.nib.com.au/.well-known/openid-configuration
  request_parameter_supported: false
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
  sources:
  - well-known/nib-health-funds-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_alg_values_supported:
  - RS256
  - RS384
  - PS256
  type: openIdConnect
- discovery_status: 200
  issuer: https://id.nib.co.nz/
  name: nib New Zealand member identity (Auth0 OIDC)
  note: Same Auth0 shape and same identity-only scope set as the Australian tenant.
  openIdConnectUrl: https://id.nib.co.nz/.well-known/openid-configuration
  sources:
  - well-known/nib-health-funds-nz-openid-configuration.json
  type: openIdConnect
- host: https://api-gateway.nib.com.au
  name: nib API gateway (undocumented)
  note: 'Real first-party AWS API Gateway named in nib''s own Content-Security-Policy.

    Anonymous requests to /, /openapi.json, /swagger.json, /docs, /graphql and

    every /.well-known/ path return HTTP 403 {"message":"Forbidden"}. No

    WWW-Authenticate challenge, no auth metadata, no public documentation, so

    the credential model cannot be determined without a partner agreement.

    '
  sources:
  - review.yml
  type: unknown
slug: nib-health-funds-authentication
source_filename: nib-health-funds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://id.nib.com.au/.well-known/openid-configuration\ndocs: https://id.nib.com.au/.well-known/openid-configuration\nnote: |\n  nib publishes no OpenAPI, so this profile is not derived from a spec. It is\n  read verbatim from the anonymously-readable OpenID Connect discovery\n  documents of nib's Auth0 member identity tenants (Australia and New Zealand),\n  plus live probes of the first-party API gateway.\n\n  Scope: this is CONSUMER SIGN-IN identity, not a partner/product API\n  authorization surface. No product, policy, claims, or partner scopes are\n  published anywhere. Provider-side (healthcare practitioner) access to nib is\n  a username/password portal login at the nib HCP portal, and electronic\n  claiming runs over third-party HICAPS and HealthPoint terminals.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, password, deviceCode,\n    tokenExchange,\
  \ jwtBearer]\n  product_api_auth: undocumented\nschemes:\n- name: nib Australia member identity (Auth0 OIDC)\n  type: openIdConnect\n  issuer: https://id.nib.com.au/\n  openIdConnectUrl: https://id.nib.com.au/.well-known/openid-configuration\n  discovery_status: 200\n  sources: [well-known/nib-health-funds-openid-configuration.json]\n  endpoints:\n    authorization: https://id.nib.com.au/authorize\n    token: https://id.nib.com.au/oauth/token\n    userinfo: https://id.nib.com.au/userinfo\n    revocation: https://id.nib.com.au/oauth/revoke\n    registration: https://id.nib.com.au/oidc/register\n    device_authorization: https://id.nib.com.au/oauth/device/code\n    backchannel_authentication: https://id.nib.com.au/bc-authorize\n    mfa_challenge: https://id.nib.com.au/mfa/challenge\n    jwks: https://id.nib.com.au/.well-known/jwks.json\n    global_token_revocation: https://id.nib.com.au/oauth/global-token-revocation/connection/{connectionName}\n  grant_types_supported:\n  - client_credentials\n\
  \  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types_supported: [code, token, id_token, code token, code id_token, token\n      id_token, code token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post,\n    private_key_jwt, none]\n  token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, PS256]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  code_challenge_methods_supported: [S256, plain]\n  dpop_signing_alg_values_supported:\
  \ [ES256]\n  subject_types_supported: [public]\n  backchannel_logout_supported: true\n  backchannel_token_delivery_modes_supported: [poll]\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n  claims_supported: [aud, auth_time, created_at, email, email_verified, exp, family_name,\n    given_name, iat, identities, iss, name, nickname, phone_number, picture, sub]\n  jwks:\n    file: well-known/nib-health-funds-jwks.json\n    keys: 2\n    algs: [RS256]\n- name: nib New Zealand member identity (Auth0 OIDC)\n  type: openIdConnect\n  issuer: https://id.nib.co.nz/\n  openIdConnectUrl: https://id.nib.co.nz/.well-known/openid-configuration\n  discovery_status: 200\n  sources: [well-known/nib-health-funds-nz-openid-configuration.json]\n  note: Same Auth0 shape and same identity-only scope set as the Australian tenant.\n- name: nib API gateway (undocumented)\n  type: unknown\n  host: https://api-gateway.nib.com.au\n  sources: [review.yml]\n  note: |\n    Real first-party\
  \ AWS API Gateway named in nib's own Content-Security-Policy.\n    Anonymous requests to /, /openapi.json, /swagger.json, /docs, /graphql and\n    every /.well-known/ path return HTTP 403 {\"message\":\"Forbidden\"}. No\n    WWW-Authenticate challenge, no auth metadata, no public documentation, so\n    the credential model cannot be determined without a partner agreement.\nprobes:\n- url: https://id.nib.com.au/.well-known/openid-configuration\n  status: 200\n- url: https://id.nib.com.au/.well-known/oauth-authorization-server\n  status: 200\n- url: https://id.nib.com.au/.well-known/jwks.json\n  status: 200\n- url: https://id.nib.com.au/userinfo\n  status: 401\n  note: Anonymous request rejected — confirms a live protected resource.\n- url: https://id.nib.com.au/oauth/token\n  status: 401\n  note: Anonymous POST rejected.\n- url: https://id.nib.co.nz/.well-known/openid-configuration\n  status: 200\n- url: https://api-gateway.nib.com.au/.well-known/oauth-protected-resource\n  status: 403\n\
  related:\n  scopes: scopes/nib-health-funds-scopes.yml\n  well_known: well-known/nib-health-funds-well-known.yml\n  conformance: conformance/nib-health-funds-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nib-health-funds/refs/heads/main/authentication/nib-health-funds-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Insurance
- Australia
- Health Insurance
- Carrier
- Claims
- Private Health Insurance
- Travel Insurance
- New Zealand
- NDIS
- Partner Gated
---
