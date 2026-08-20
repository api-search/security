---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cytora Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- deviceCode
- refreshToken
- tokenExchange
- jwtBearer
overview: Cytora secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, deviceCode, refreshToken, tokenExchange, and jwtBearer flow(s).
provider_name: Cytora
provider_slug: cytora
scheme_count: 2
schemes:
- authorization_grant_profiles:
  - urn:ietf:params:oauth:grant-profile:id-jag
  backchannel_logout_supported: true
  claims:
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
  dpop_signing_algs:
  - ES256
  endpoints:
    authorization: https://auth.cytora.com/authorize
    backchannel_authentication: https://auth.cytora.com/bc-authorize
    device_authorization: https://auth.cytora.com/oauth/device/code
    jwks: https://auth.cytora.com/.well-known/jwks.json
    mfa_challenge: https://auth.cytora.com/mfa/challenge
    registration: https://auth.cytora.com/oidc/register
    revocation: https://auth.cytora.com/oauth/revoke
    token: https://auth.cytora.com/oauth/token
    userinfo: https://auth.cytora.com/userinfo
  flows:
  - flow: clientCredentials
    grant: client_credentials
    use: machine-to-machine partner and customer integrations
  - flow: authorizationCode
    grant: authorization_code
    pkce:
    - S256
    - plain
    use: interactive Risk Console sign-in (https://uwp.cytora.com)
  - flow: refreshToken
    grant: refresh_token
  - flow: deviceCode
    grant: urn:ietf:params:oauth:grant-type:device_code
  - flow: tokenExchange
    grant: urn:ietf:params:oauth:grant-type:token-exchange
  - flow: jwtBearer
    grant: urn:ietf:params:oauth:grant-type:jwt-bearer
  - flow: password
    grant: password
    note: legacy ROPC grant advertised by the tenant
  - flow: implicit
    grant: implicit
    note: legacy grant advertised by the tenant
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.cytora.com/
  name: CytoraOAuth2
  provider: Auth0 (EU tenant cytora-prod.eu.auth0.com)
  request_parameter_supported: false
  request_uri_parameter_supported: false
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/cytora-openid-configuration.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  type: oauth2
- name: CytoraOIDC
  openIdConnectUrl: https://auth.cytora.com/.well-known/openid-configuration
  sources:
  - well-known/cytora-openid-configuration.json
  type: openIdConnect
slug: cytora-authentication
source_filename: cytora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.cytora.com/.well-known/openid-configuration\ndocs: https://auth.cytora.com/.well-known/openid-configuration\nnote: >-\n  Cytora publishes no OpenAPI, so this profile is read directly from the live\n  OpenID Connect discovery document of Cytora's identity provider rather than\n  derived from securitySchemes. Partner and customer integrations against\n  api.cytora.com are provisioned per contract; client credentials cannot be\n  obtained self-serve.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode, deviceCode, refreshToken, tokenExchange, jwtBearer]\n  bearer_token: JWT (RS256)\n  self_serve: false\nschemes:\n- name: CytoraOAuth2\n  type: oauth2\n  provider: Auth0 (EU tenant cytora-prod.eu.auth0.com)\n  issuer: https://auth.cytora.com/\n  sources: [well-known/cytora-openid-configuration.json]\n  endpoints:\n    authorization: https://auth.cytora.com/authorize\n\
  \    token: https://auth.cytora.com/oauth/token\n    device_authorization: https://auth.cytora.com/oauth/device/code\n    userinfo: https://auth.cytora.com/userinfo\n    revocation: https://auth.cytora.com/oauth/revoke\n    jwks: https://auth.cytora.com/.well-known/jwks.json\n    registration: https://auth.cytora.com/oidc/register\n    backchannel_authentication: https://auth.cytora.com/bc-authorize\n    mfa_challenge: https://auth.cytora.com/mfa/challenge\n  flows:\n  - flow: clientCredentials\n    grant: client_credentials\n    use: machine-to-machine partner and customer integrations\n  - flow: authorizationCode\n    grant: authorization_code\n    pkce: [S256, plain]\n    use: interactive Risk Console sign-in (https://uwp.cytora.com)\n  - flow: refreshToken\n    grant: refresh_token\n  - flow: deviceCode\n    grant: urn:ietf:params:oauth:grant-type:device_code\n  - flow: tokenExchange\n    grant: urn:ietf:params:oauth:grant-type:token-exchange\n  - flow: jwtBearer\n    grant: urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  - flow: password\n    grant: password\n    note: legacy ROPC grant advertised by the tenant\n  - flow: implicit\n    grant: implicit\n    note: legacy grant advertised by the tenant\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  token_endpoint_auth_signing_algs: [RS256, RS384, PS256]\n  id_token_signing_algs: [HS256, RS256, PS256]\n  dpop_signing_algs: [ES256]\n  response_types: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  response_modes: [query, fragment, form_post]\n  subject_types: [public]\n  claims: [aud, auth_time, created_at, email, email_verified, exp, family_name,\n    given_name, iat, identities, iss, name, nickname, phone_number, picture, sub]\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n  backchannel_logout_supported: true\n  authorization_grant_profiles: [urn:ietf:params:oauth:grant-profile:id-jag]\n- name: CytoraOIDC\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://auth.cytora.com/.well-known/openid-configuration\n  sources: [well-known/cytora-openid-configuration.json]\nclient_evidence:\n  source: https://uwp.cytora.com (Risk Console SPA JavaScript bundles)\n  observed:\n  - auth0-spa-js is the browser authentication library\n  - requests carry an Authorization header (bearer)\n  - no API key header or query parameter observed anywhere in the client\ngaps:\n- No public authentication guide; the ReadMe documentation host is password-protected.\n- No self-serve credential issuance; no developer signup exists.\n- No product/resource scopes published anonymously (see scopes/cytora-scopes.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cytora/refs/heads/main/authentication/cytora-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Insurance
- United Kingdom
- Insurtech
- Commercial Insurance
- Underwriting
- Claims
- Risk Data
- Property and Casualty
- Reinsurance
- Brokers
- Submission Intake
- Document AI
---
