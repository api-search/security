---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Clarify Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clarify Health declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Clarify Health
provider_slug: clarify-health
scheme_count: 0
schemes: []
slug: clarify-health-authentication
source_filename: clarify-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  https://auth.clarifyhealth.com/.well-known/openid-configuration and\n  https://okta.clarifyhealth.com/.well-known/openid-configuration (both HTTP 200,\n  fetched 2026-08-15)\nscope_of_this_document: >-\n  Clarify Health publishes no public API and no developer authentication guide. What it\n  does publish, anonymously and machine-readably, are two OpenID Connect discovery\n  documents on hosts it controls. They describe how a human or a machine authenticates\n  INTO the Clarify Atlas / Meridian platform — they are not the authentication profile of\n  a product API, because no product API is published. Everything below is read verbatim\n  from those two documents; nothing is inferred.\nproviders:\n- name: Auth0 tenant (customer + workforce sign-in)\n  issuer: https://auth.clarifyhealth.com/\n  discovery: https://auth.clarifyhealth.com/.well-known/openid-configuration\n  file: ../well-known/clarify-health-auth-openid-configuration.json\n\
  \  http_status: 200\n  endpoints:\n    authorization: https://auth.clarifyhealth.com/authorize\n    token: https://auth.clarifyhealth.com/oauth/token\n    userinfo: https://auth.clarifyhealth.com/userinfo\n    jwks: https://auth.clarifyhealth.com/.well-known/jwks.json\n    revocation: https://auth.clarifyhealth.com/oauth/revoke\n    registration: https://auth.clarifyhealth.com/oidc/register\n    device_authorization: https://auth.clarifyhealth.com/oauth/device/code\n    backchannel_authentication: https://auth.clarifyhealth.com/bc-authorize\n    mfa_challenge: https://auth.clarifyhealth.com/mfa/challenge\n  schemes:\n  - type: openIdConnect\n    name: OpenID Connect\n    id_token_signing: [HS256, RS256, PS256]\n  - type: oauth2\n    flows: [authorization_code, client_credentials, refresh_token, password, implicit, device_code, token_exchange, jwt_bearer]\n    note: >-\n      client_credentials is advertised, which means machine-to-machine tokens are issuable\n      against this tenant\
  \ — but no resource server / audience is publicly documented.\n  pkce:\n    supported: true\n    methods: [S256, plain]\n    note: '\"plain\" is still advertised alongside S256.'\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  mfa: true\n  dpop:\n    supported: true\n    algs: [ES256]\n  backchannel_logout: true\n  scopes_supported: [openid, profile, offline_access, name, given_name, family_name, nickname,\n    email, email_verified, picture, created_at, identities, phone, address]\n  note: >-\n    Only standard OIDC identity scopes are advertised. There are no Clarify-specific\n    resource scopes in the discovery document, which is consistent with there being no\n    published product API to scope.\n- name: Okta org authorization server\n  issuer: https://okta.clarifyhealth.com\n  discovery: https://okta.clarifyhealth.com/.well-known/openid-configuration\n  file: ../well-known/clarify-health-okta-openid-configuration.json\n  http_status:\
  \ 200\n  endpoints:\n    authorization: https://okta.clarifyhealth.com/oauth2/v1/authorize\n    token: https://okta.clarifyhealth.com/oauth2/v1/token\n    userinfo: https://okta.clarifyhealth.com/oauth2/v1/userinfo\n    jwks: https://okta.clarifyhealth.com/oauth2/v1/keys\n    introspection: https://okta.clarifyhealth.com/oauth2/v1/introspect\n    revocation: https://okta.clarifyhealth.com/oauth2/v1/revoke\n    end_session: https://okta.clarifyhealth.com/oauth2/v1/logout\n    registration: https://okta.clarifyhealth.com/oauth2/v1/clients\n    device_authorization: https://okta.clarifyhealth.com/oauth2/v1/device/authorize\n    pushed_authorization_request: https://okta.clarifyhealth.com/oauth2/v1/par\n  schemes:\n  - type: openIdConnect\n    name: OpenID Connect\n    id_token_signing: [RS256]\n    id_token_encryption:\n      alg: [RSA-OAEP-256, RSA-OAEP-384, RSA-OAEP-512]\n      enc: [A256GCM]\n  - type: oauth2\n    flows: [authorization_code, implicit, refresh_token, password, device_code,\
  \ ciba, okta_otp, okta_oob]\n  pkce:\n    supported: true\n    methods: [S256]\n    note: S256 only — no \"plain\" downgrade.\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt,\n    private_key_jwt, none]\n  par: true\n  dpop:\n    supported: true\n    algs: [RS256, RS384, RS512, ES256, ES384, ES512]\n  scopes_supported: [openid, email, profile, address, phone, offline_access, groups]\n  custom_authorization_servers:\n    public: false\n    note: >-\n      /oauth2/default/.well-known/openid-configuration returns 401 E0000015, so any\n      Clarify-specific API scopes that exist on a custom authorization server are not\n      anonymously discoverable.\napi_keys:\n  documented: false\n  note: No public API key issuance, key prefix, or credential documentation was found.\nmutual_tls:\n  documented: false\nfindings:\n- Two independent identity providers are live for one company (Auth0 for the platform, Okta\n  for the org) — a normal split, but consumers\
  \ of a future Clarify API would need to be\n  told which issuer is authoritative.\n- Both issuers advertise DPoP, PKCE, and dynamic client registration; neither publishes a\n  resource-server audience, so there is no way for an outside integrator to obtain a token\n  that is good for anything.\n- The Auth0 tenant still advertises the deprecated `password` and `implicit` grants and\n  `plain` PKCE.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarify-health/refs/heads/main/authentication/clarify-health-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Health Tech
- Healthcare Analytics
- Health Data
- Outcomes
- Referral Intelligence
- Payers
- Life Sciences
---
