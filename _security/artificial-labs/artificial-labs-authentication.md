---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Artificial Labs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- refreshToken
- deviceCode
- tokenExchange
- jwtBearer
overview: Artificial Labs secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, refreshToken, deviceCode, tokenExchange, and jwtBearer flow(s).
provider_name: Artificial Labs
provider_slug: artificial-labs
scheme_count: 1
schemes:
- backchannel_logout_supported: true
  code_challenge_methods_supported:
  - S256
  - plain
  dpop_signing_alg_values_supported:
  - ES256
  endpoints:
    authorization: https://auth.artificialos.com/authorize
    backchannel_authentication: https://auth.artificialos.com/bc-authorize
    device_authorization: https://auth.artificialos.com/oauth/device/code
    global_token_revocation: https://auth.artificialos.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.artificialos.com/.well-known/jwks.json
    mfa_challenge: https://auth.artificialos.com/mfa/challenge
    registration: https://auth.artificialos.com/oidc/register
    revocation: https://auth.artificialos.com/oauth/revoke
    token: https://auth.artificialos.com/oauth/token
    userinfo: https://auth.artificialos.com/userinfo
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
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.artificialos.com/
  mfa: true
  name: Auth0 OpenID Connect
  openIdConnectUrl: https://auth.artificialos.com/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/artificial-labs-openid-configuration.json
  tenant: artificial.uk.auth0.com
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: artificial-labs-authentication
source_filename: artificial-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.artificialos.com/.well-known/openid-configuration\ndocs: https://docs.artificial.io/docs-site/\nnote: |\n  Artificial Labs publishes no OpenAPI, so this profile is not derived from\n  securitySchemes — it is read verbatim from the one authentication surface the\n  company does expose anonymously: the Auth0 UK tenant that fronts both the\n  product documentation (via oauth2-proxy) and, by inference, the platform\n  itself. Partner API credentials for Smart Underwriting, Smart Placement and\n  Contract Builder are issued out of band under a contract; there is no public\n  self-serve key issuance and no documented API-key scheme.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - refreshToken\n  - deviceCode\n  - tokenExchange\n  - jwtBearer\n  public_self_serve_signup: false\n  credential_issuance: out\
  \ of band, under partner/customer contract\nschemes:\n- name: Auth0 OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.artificialos.com/.well-known/openid-configuration\n  issuer: https://auth.artificialos.com/\n  tenant: artificial.uk.auth0.com\n  sources:\n  - well-known/artificial-labs-openid-configuration.json\n  endpoints:\n    authorization: https://auth.artificialos.com/authorize\n    token: https://auth.artificialos.com/oauth/token\n    userinfo: https://auth.artificialos.com/userinfo\n    jwks: https://auth.artificialos.com/.well-known/jwks.json\n    revocation: https://auth.artificialos.com/oauth/revoke\n    registration: https://auth.artificialos.com/oidc/register\n    device_authorization: https://auth.artificialos.com/oauth/device/code\n    backchannel_authentication: https://auth.artificialos.com/bc-authorize\n    mfa_challenge: https://auth.artificialos.com/mfa/challenge\n    global_token_revocation: https://auth.artificialos.com/oauth/global-token-revocation/connection/{connectionName}\n\
  \  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_alg_values_supported:\n  - ES256\n  backchannel_logout_supported:\
  \ true\n  mfa: true\nobserved_clients:\n- name: docs.artificial.io (oauth2-proxy)\n  client_id: doz61CY73D2YYnTftWiDXl5j31Npm7b7\n  flow: authorizationCode\n  scope: openid profile email\n  redirect_uri: https://docs.artificial.io/oauth2/callback\n  entry_point: https://docs.artificial.io/oauth2/start\n  note: Observed on the 302 from every gated documentation path. Public client id\n    only; no secret is exposed.\ngaps:\n- No public API-key issuance or API-key documentation.\n- No published mTLS / FAPI client-authentication guidance, although private_key_jwt\n  and DPoP (ES256) are advertised by the tenant.\n- No published domain/product scopes — only standard OIDC scopes (see\n  scopes/artificial-labs-scopes.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artificial-labs/refs/heads/main/authentication/artificial-labs-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Insurance
- United Kingdom
- Insurtech
- Underwriting
- Reinsurance
- Specialty Insurance
- London Market
- Lloyd's of London
- Broker
- Policy Administration
- ACORD
- Algorithmic Underwriting
---
