---
anonymous_access: false
api_key_in: []
auth_types: []
description: F&G Annuities & Life (FGL Holdings) publishes no public product API and no developer authentication guide. It does operate a real, first-party OpenID Connect authorization server at auth.fglife.com — an Auth0 custom domain fronting the prod.fglife.auth0.com tenant — which serves a complete OIDC discovery document anonymously. Everything below is read verbatim from that document, not from prose. The authorization server gates the SalesLink financial-professional portal; access is granted through an IMO/broker-dealer appointment, not self-service registration, so no member of the public can obtain a client credential.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Fgl Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: FGL Holdings declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FGL Holdings
provider_slug: fgl-holdings
scheme_count: 2
schemes:
- bearer_format: JWT
  description: 'Authorization Code with PKCE. Observed live: saleslink.fglife.com issues a 302 to https://auth.fglife.com/authorize with response_type=code, code_challenge_method=S256, response_mode=form_post and scope "offline_access openid profile email".'
  evidence: https://saleslink.fglife.com/ (HTTP 302, Location header)
  in: header
  name: oidc_authorization_code_pkce
  openid_connect_url: https://auth.fglife.com/.well-known/openid-configuration
  public_client_registration: false
  scheme: bearer
  type: openIdConnect
- description: Declared in grant_types_supported. No public client registration; credentials are issued to appointed distribution partners only.
  flow: clientCredentials
  gated: true
  name: oauth2_client_credentials
  token_endpoint: https://auth.fglife.com/oauth/token
  type: oauth2
slug: fgl-holdings-authentication
source_filename: fgl-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://auth.fglife.com/.well-known/openid-configuration\nprovider: FGL Holdings\nproviderId: fgl-holdings\ndescription: >-\n  F&G Annuities & Life (FGL Holdings) publishes no public product API and no developer authentication\n  guide. It does operate a real, first-party OpenID Connect authorization server at auth.fglife.com — an\n  Auth0 custom domain fronting the prod.fglife.auth0.com tenant — which serves a complete OIDC discovery\n  document anonymously. Everything below is read verbatim from that document, not from prose. The\n  authorization server gates the SalesLink financial-professional portal; access is granted through an\n  IMO/broker-dealer appointment, not self-service registration, so no member of the public can obtain a\n  client credential.\nnotes: >-\n  This artifact profiles an IDENTITY surface, not a product API. Recording it does not assert that F&G\n  offers a callable public API — it does not. See conventions/\
  \ and the apis.yml x-coverage block.\nissuer: https://auth.fglife.com/\nalternate_issuer: https://prod.fglife.auth0.com/\nprovider_platform: Auth0 (custom domain)\nschemes:\n  - name: oidc_authorization_code_pkce\n    type: openIdConnect\n    in: header\n    scheme: bearer\n    bearer_format: JWT\n    openid_connect_url: https://auth.fglife.com/.well-known/openid-configuration\n    description: >-\n      Authorization Code with PKCE. Observed live: saleslink.fglife.com issues a 302 to\n      https://auth.fglife.com/authorize with response_type=code, code_challenge_method=S256,\n      response_mode=form_post and scope \"offline_access openid profile email\".\n    evidence: https://saleslink.fglife.com/ (HTTP 302, Location header)\n    public_client_registration: false\n  - name: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://auth.fglife.com/oauth/token\n    description: >-\n      Declared in grant_types_supported. No public client registration;\
  \ credentials are issued to\n      appointed distribution partners only.\n    gated: true\nendpoints:\n  authorization: https://auth.fglife.com/authorize\n  token: https://auth.fglife.com/oauth/token\n  userinfo: https://auth.fglife.com/userinfo\n  jwks_uri: https://auth.fglife.com/.well-known/jwks.json\n  revocation: https://auth.fglife.com/oauth/revoke\n  registration: https://auth.fglife.com/oidc/register\n  device_authorization: https://auth.fglife.com/oauth/device/code\n  backchannel_authentication: https://auth.fglife.com/bc-authorize\n  mfa_challenge: https://auth.fglife.com/mfa/challenge\n  global_token_revocation: https://auth.fglife.com/oauth/global-token-revocation/connection/{connectionName}\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n\
  \  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\ncode_challenge_methods_supported:\n  - S256\n  - plain\nid_token_signing_alg_values_supported:\n  - RS256\n  - PS256\n  - HS256\ndpop_signing_alg_values_supported:\n  - ES256\nmfa:\n  supported: true\n  evidence: mfa_challenge endpoint plus mfa-oob / mfa-otp / mfa-recovery-code grant types\nlogout:\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\ngaps:\n  - No public developer documentation for authentication — no auth guide, no key-issuance page.\n  - No client registration open to the public; registration_endpoint exists but the portal is appointment-gated.\n  - No /.well-known/oauth-protected-resource anywhere on the estate (404\
  \ on auth.fglife.com and api.fglife.com).\n  - plain is advertised alongside S256 in code_challenge_methods_supported (Auth0 tenant default).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fgl-holdings/refs/heads/main/authentication/fgl-holdings-authentication.yml
summary_line: 2 schemes
tags:
- Insurance
- Annuities
- Financial-Services
- Life Insurance
- Retirement
- Pension-Risk-Transfer
---
