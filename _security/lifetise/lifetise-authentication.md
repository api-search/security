---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lifetise Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- password
- implicit
- tokenExchange
- jwtBearer
overview: Coadjute secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, password, implicit, tokenExchange, and jwtBearer flow(s).
provider_name: Coadjute
provider_slug: lifetise
scheme_count: 3
schemes:
- backchannel_logout_supported: true
  backchannel_token_delivery_modes_supported:
  - poll
  code_challenge_methods_supported:
  - S256
  - plain
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://auth.coadjute.com/authorize
    backchannel_authentication: https://auth.coadjute.com/bc-authorize
    device_authorization: https://auth.coadjute.com/oauth/device/code
    global_token_revocation: https://auth.coadjute.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.coadjute.com/.well-known/jwks.json
    mfa_challenge: https://auth.coadjute.com/mfa/challenge
    registration: https://auth.coadjute.com/oidc/register
    revocation: https://auth.coadjute.com/oauth/revoke
    token: https://auth.coadjute.com/oauth/token
    userinfo: https://auth.coadjute.com/userinfo
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.coadjute.com/
  name: coadjute-oidc
  openIdConnectUrl: https://auth.coadjute.com/.well-known/openid-configuration
  provider: Auth0
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
  - well-known/lifetise-openid-configuration.json
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
- authorization_grant_profiles_supported:
  - urn:ietf:params:oauth:grant-profile:id-jag
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  name: coadjute-oauth2
  scopes: scopes/lifetise-scopes.yml
  sources:
  - well-known/lifetise-oauth-authorization-server.json
  type: oauth2
- evidence: 'Street''s Coadjute integration page instructs agents to email street@coadjute.com for

    a guide on "how to enable webhooks and obtain your API token" — credentials for the

    Partner Cloud API are issued by a human under a signed partner agreement. The header

    name and token format are not published anywhere public.

    Corroborated by the NeosAlpha case study describing a Kong API gateway fronting

    Coadjute''s partner APIs with an "OAuth2.0-based security model".

    '
  in: header
  name: coadjute-partner-token
  provisioning: manual
  self_serve: false
  sources:
  - https://www.street.co.uk/integrations/coadjute
  type: apiKey
slug: lifetise-authentication
source_filename: lifetise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://auth.coadjute.com/.well-known/openid-configuration\ndocs: https://www.coadjute.com/coadjute-partner-terms-of-service\nraw:\n- well-known/lifetise-openid-configuration.json\n- well-known/lifetise-oauth-authorization-server.json\n- authentication/coadjute-openid-configuration.json\nnote: |\n  Derived from the only anonymously fetchable machine-readable contract Coadjute\n  publishes: the Auth0-backed OpenID Connect discovery document on auth.coadjute.com.\n  There is no OpenAPI to derive securitySchemes from — api.coadjute.com is fully gated\n  and developer.coadjute.com returns 502 — so this profile records the identity layer as\n  advertised by the tenant plus the manually provisioned partner token path evidenced by\n  a third-party CRM integration page. Nothing here is inferred beyond those two sources.\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode,\
  \ clientCredentials, deviceCode, password, implicit, tokenExchange, jwtBearer]\n  pkce: true\n  pkce_methods: [S256, plain]\n  mfa: true\n  dpop: true\n  dynamic_client_registration: true\nschemes:\n- name: coadjute-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.coadjute.com/.well-known/openid-configuration\n  issuer: https://auth.coadjute.com/\n  provider: Auth0\n  sources: [well-known/lifetise-openid-configuration.json]\n  endpoints:\n    authorization: https://auth.coadjute.com/authorize\n    token: https://auth.coadjute.com/oauth/token\n    userinfo: https://auth.coadjute.com/userinfo\n    jwks: https://auth.coadjute.com/.well-known/jwks.json\n    registration: https://auth.coadjute.com/oidc/register\n    revocation: https://auth.coadjute.com/oauth/revoke\n    device_authorization: https://auth.coadjute.com/oauth/device/code\n    mfa_challenge: https://auth.coadjute.com/mfa/challenge\n    backchannel_authentication: https://auth.coadjute.com/bc-authorize\n    global_token_revocation:\
  \ https://auth.coadjute.com/oauth/global-token-revocation/connection/{connectionName}\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, PS256]\n  response_types_supported: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  subject_types_supported: [public]\n  code_challenge_methods_supported: [S256, plain]\n  dpop_signing_alg_values_supported: [ES256]\n  backchannel_logout_supported: true\n  backchannel_token_delivery_modes_supported: [poll]\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n- name: coadjute-oauth2\n  type: oauth2\n  sources: [well-known/lifetise-oauth-authorization-server.json]\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n\
  \  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  authorization_grant_profiles_supported:\n  - urn:ietf:params:oauth:grant-profile:id-jag\n  scopes: scopes/lifetise-scopes.yml\n- name: coadjute-partner-token\n  type: apiKey\n  in: header\n  provisioning: manual\n  self_serve: false\n  sources:\n  - https://www.street.co.uk/integrations/coadjute\n  evidence: |\n    Street's Coadjute integration page instructs agents to email street@coadjute.com for\n    a guide on \"how to enable webhooks and obtain your API token\" — credentials for the\n    Partner Cloud API are issued by a human under a signed partner\
  \ agreement. The header\n    name and token format are not published anywhere public.\n    Corroborated by the NeosAlpha case study describing a Kong API gateway fronting\n    Coadjute's partner APIs with an \"OAuth2.0-based security model\".\naccess:\n  gate: partner-only\n  self_serve_signup: false\n  what_is_required: |\n    A signed Coadjute Partner Terms of Service with an Order Form and Subscription Term.\n    There is no developer signup: every public conversion path is \"Book a demo\",\n    \"Request access\" or \"Login\".\nclaims_supported: [aud, auth_time, created_at, email, email_verified, exp, family_name,\n  given_name, iat, identities, iss, name, nickname, phone_number, picture, sub]\nprobes:\n- {url: 'https://auth.coadjute.com/.well-known/openid-configuration', status: 200}\n- {url: 'https://auth.coadjute.com/.well-known/oauth-authorization-server', status: 200}\n- {url: 'https://auth.coadjute.com/.well-known/jwks.json', status: 200, saved: false, note: rotating key material}\n\
  - {url: 'https://api.coadjute.com/.well-known/openid-configuration', status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifetise/refs/heads/main/authentication/lifetise-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Transactions
- Conveyancing
- AML
- Compliance
- Distributed Ledger
- Estate Agents
- Mortgage
---
