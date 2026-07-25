---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tal Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refresh_token
- password
- device_code
- ciba
overview: TAL secures its APIs with openIdConnect, oauth2, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refresh_token, password, device_code, and ciba flow(s).
provider_name: TAL
provider_slug: tal-australia
scheme_count: 5
schemes:
- code_challenge_methods:
  - S256
  dpop_signing_alg:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://login.talpartner.tal.com.au/oauth2/v1/authorize
    device_authorization: https://login.talpartner.tal.com.au/oauth2/v1/device/authorize
    end_session: https://login.talpartner.tal.com.au/oauth2/v1/logout
    introspection: https://login.talpartner.tal.com.au/oauth2/v1/introspect
    jwks: https://login.talpartner.tal.com.au/oauth2/v1/keys
    pushed_authorization_request: https://login.talpartner.tal.com.au/oauth2/v1/par
    registration: https://login.talpartner.tal.com.au/oauth2/v1/clients
    revocation: https://login.talpartner.tal.com.au/oauth2/v1/revoke
    token: https://login.talpartner.tal.com.au/oauth2/v1/token
    userinfo: https://login.talpartner.tal.com.au/oauth2/v1/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_encryption_alg:
  - RSA-OAEP-256
  - RSA-OAEP-384
  - RSA-OAEP-512
  id_token_signing_alg:
  - RS256
  issuer: https://login.talpartner.tal.com.au
  name: talpartner-oidc
  openIdConnectUrl: https://login.talpartner.tal.com.au/.well-known/openid-configuration
  purpose: Partner / distributor sign-in for TAL partner applications
  request_object_supported: true
  response_types:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  sources:
  - well-known/tal-australia-talpartner-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  vendor: Okta (org talpartner-au.okta.com)
- code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  issuer: https://auth.acp.tal.com.au
  name: acp-oidc
  openIdConnectUrl: https://auth.acp.tal.com.au/.well-known/openid-configuration
  purpose: Identity for acp.tal.com.au
  sources:
  - well-known/tal-australia-acp-openid-configuration.json
  type: openIdConnect
  vendor: Okta
- code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://auth.claimsassist.tal.com.au
  name: claimsassist-oidc
  openIdConnectUrl: https://auth.claimsassist.tal.com.au/.well-known/openid-configuration
  purpose: Identity for TAL Claims Assist (claimassist.tal.com.au) and its EFT / group-claims / TFN APIs
  sources:
  - well-known/tal-australia-claimsassist-openid-configuration.json
  type: openIdConnect
  vendor: Okta
- evidence: 'HTTP 401 with WWW-Authenticate: Bearer realm="app-b2bcommon-prodmel.azurewebsites.net" from https://common.glsb2b.tal.com.au/ on 2026-07-25 (ASP.NET on Azure App Service). Every path probed under that host returns 401 to an anonymous caller, including /swagger, /swagger/v1/swagger.json and /openapi.json.'
  name: glsb2b-bearer
  purpose: TAL Group Life B2B (glsb2b) partner API estate
  scheme: bearer
  sources:
  - live probe
  type: http
- evidence: Sitecore extranet login; unknown paths 302 to /404?item=...&user=extranet%5cAnonymous&site=TAC. No OIDC discovery served.
  name: adviser-centre-session
  purpose: TAL Adviser Centre extranet (adviser.tal.com.au)
  scheme: cookie
  sources:
  - review.yml
  type: session
slug: tal-australia-authentication
source_filename: tal-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://login.talpartner.tal.com.au/.well-known/openid-configuration\ndocs: null\nnote: |\n  TAL publishes no OpenAPI, so this profile is built from live, anonymous\n  OpenID Connect discovery documents on TAL's own identity hosts plus the\n  WWW-Authenticate challenges returned by TAL's partner API hosts. Every value\n  below was observed on 2026-07-25; nothing is inferred from marketing copy.\nsummary:\n  types: [openIdConnect, oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, refresh_token, password, device_code,\n    ciba]\n  pkce: S256\n  public_registration: false\n  gated: true\nschemes:\n- name: talpartner-oidc\n  type: openIdConnect\n  issuer: https://login.talpartner.tal.com.au\n  openIdConnectUrl: https://login.talpartner.tal.com.au/.well-known/openid-configuration\n  vendor: Okta (org talpartner-au.okta.com)\n  purpose: Partner / distributor sign-in for TAL partner applications\n  endpoints:\n\
  \    authorization: https://login.talpartner.tal.com.au/oauth2/v1/authorize\n    token: https://login.talpartner.tal.com.au/oauth2/v1/token\n    userinfo: https://login.talpartner.tal.com.au/oauth2/v1/userinfo\n    jwks: https://login.talpartner.tal.com.au/oauth2/v1/keys\n    introspection: https://login.talpartner.tal.com.au/oauth2/v1/introspect\n    revocation: https://login.talpartner.tal.com.au/oauth2/v1/revoke\n    end_session: https://login.talpartner.tal.com.au/oauth2/v1/logout\n    registration: https://login.talpartner.tal.com.au/oauth2/v1/clients\n    device_authorization: https://login.talpartner.tal.com.au/oauth2/v1/device/authorize\n    pushed_authorization_request: https://login.talpartner.tal.com.au/oauth2/v1/par\n  grant_types: [authorization_code, implicit, refresh_token, password,\n    'urn:ietf:params:oauth:grant-type:device_code', 'urn:openid:params:grant-type:ciba']\n  response_types: [code, id_token, code id_token, code token, id_token token,\n    code id_token token]\n\
  \  token_endpoint_auth_methods: [client_secret_basic, client_secret_post,\n    client_secret_jwt, private_key_jwt, none]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  id_token_encryption_alg: [RSA-OAEP-256, RSA-OAEP-384, RSA-OAEP-512]\n  dpop_signing_alg: [RS256, RS384, RS512, ES256, ES384, ES512]\n  request_object_supported: true\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json]\n- name: acp-oidc\n  type: openIdConnect\n  issuer: https://auth.acp.tal.com.au\n  openIdConnectUrl: https://auth.acp.tal.com.au/.well-known/openid-configuration\n  vendor: Okta\n  purpose: Identity for acp.tal.com.au\n  grant_types: [authorization_code, implicit, refresh_token, password,\n    'urn:ietf:params:oauth:grant-type:device_code', 'urn:openid:params:grant-type:ciba']\n  code_challenge_methods: [S256]\n  sources: [well-known/tal-australia-acp-openid-configuration.json]\n- name: claimsassist-oidc\n  type: openIdConnect\n  issuer: https://auth.claimsassist.tal.com.au\n\
  \  openIdConnectUrl: https://auth.claimsassist.tal.com.au/.well-known/openid-configuration\n  vendor: Okta\n  purpose: Identity for TAL Claims Assist (claimassist.tal.com.au) and its\n    EFT / group-claims / TFN APIs\n  grant_types: [authorization_code, implicit, refresh_token, password,\n    'urn:ietf:params:oauth:grant-type:device_code']\n  code_challenge_methods: [S256]\n  sources: [well-known/tal-australia-claimsassist-openid-configuration.json]\n- name: glsb2b-bearer\n  type: http\n  scheme: bearer\n  purpose: TAL Group Life B2B (glsb2b) partner API estate\n  evidence: 'HTTP 401 with WWW-Authenticate: Bearer realm=\"app-b2bcommon-prodmel.azurewebsites.net\"\n    from https://common.glsb2b.tal.com.au/ on 2026-07-25 (ASP.NET on Azure App\n    Service). Every path probed under that host returns 401 to an anonymous\n    caller, including /swagger, /swagger/v1/swagger.json and /openapi.json.'\n  sources: [live probe]\n- name: adviser-centre-session\n  type: session\n  scheme: cookie\n\
  \  purpose: TAL Adviser Centre extranet (adviser.tal.com.au)\n  evidence: Sitecore extranet login; unknown paths 302 to\n    /404?item=...&user=extranet%5cAnonymous&site=TAC. No OIDC discovery served.\n  sources: [review.yml]\nonboarding:\n  self_serve: false\n  note: |\n    There is no public client registration, no developer key issuance and no\n    published credential flow. Access to every TAL API host observed is granted\n    through a bilateral partner agreement (adviser software vendors, super-fund\n    administrators, payroll/embedded distributors). The Okta dynamic client\n    registration endpoint is advertised in discovery but is an Okta org default,\n    not an open self-service path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tal-australia/refs/heads/main/authentication/tal-australia-authentication.yml
summary_line: openIdConnect/oauth2/http · 5 schemes
tags:
- Insurance
- Australia
- Life Insurance
- Income Protection
- Group Insurance
- Superannuation
- Underwriting
- Claims
- Carrier
- Embedded Insurance
- Partner Gated
- No Public API
- OpenID Connect
- GraphQL
- Identity
---
