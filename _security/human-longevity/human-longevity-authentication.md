---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Human Longevity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Human Longevity declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Human Longevity
provider_slug: human-longevity
scheme_count: 1
schemes:
- audience_note: Read from the Auth0 SDK configuration embedded in the portal's own main.js bundle (https://portal.humanlongevity.com/main.aac5aadc52a10f4b.js). This is an OAuth audience identifier for the portal's private backend API. That backend publishes no contract and no documentation, and the hli.com host that the identifier is named after does not resolve to a Human Longevity property, so it is recorded as an identifier only — never as a callable base URL.
  audiences_observed:
  - https://client-portal.hli.com
  description: OpenID Connect / OAuth 2.0 authorization server for the Human Longevity client portal (portal.humanlongevity.com) and the HLI mobile app. Access is limited to HLI clinic clients; there is no self-service developer registration.
  endpoints:
    authorization: https://auth.humanlongevity.com/authorize
    device_authorization: https://auth.humanlongevity.com/oauth/device/code
    dynamic_client_registration: https://auth.humanlongevity.com/oidc/register
    jwks: https://auth.humanlongevity.com/.well-known/jwks.json
    mfa_challenge: https://auth.humanlongevity.com/mfa/challenge
    revocation: https://auth.humanlongevity.com/oauth/revoke
    token: https://auth.humanlongevity.com/oauth/token
    userinfo: https://auth.humanlongevity.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id: hli_portal_oidc
  id_token_signing_algs:
  - RS256
  - PS256
  - HS256
  mfa:
    evidence: mfa_challenge_endpoint and the four http://auth0.com/oauth/grant-type/mfa-* grant types are advertised in the discovery document.
    supported: true
  openIdConnectUrl: https://auth.humanlongevity.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: human-longevity-authentication
source_filename: human-longevity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://auth.humanlongevity.com/.well-known/openid-configuration\nscope: >-\n  This profile describes the ONLY authentication surface Human Longevity publishes: the OpenID\n  Connect authorization server that fronts the HLI client portal and mobile app. Human Longevity\n  publishes no public API, no developer program and no API key issuance, so there is no\n  developer-facing authentication documentation to profile. Everything below was read from the\n  provider's own machine-readable discovery document, not from prose.\nsummary:\n  public_api_authentication: none-published\n  end_user_authentication: openid-connect\n  provider: Auth0 (custom domain on the company's own humanlongevity.com apex)\nissuer: https://auth.humanlongevity.com/\nschemes:\n- id: hli_portal_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.humanlongevity.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect / OAuth 2.0\
  \ authorization server for the Human Longevity client portal\n    (portal.humanlongevity.com) and the HLI mobile app. Access is limited to HLI clinic clients;\n    there is no self-service developer registration.\n  endpoints:\n    authorization: https://auth.humanlongevity.com/authorize\n    token: https://auth.humanlongevity.com/oauth/token\n    userinfo: https://auth.humanlongevity.com/userinfo\n    jwks: https://auth.humanlongevity.com/.well-known/jwks.json\n    revocation: https://auth.humanlongevity.com/oauth/revoke\n    device_authorization: https://auth.humanlongevity.com/oauth/device/code\n    dynamic_client_registration: https://auth.humanlongevity.com/oidc/register\n    mfa_challenge: https://auth.humanlongevity.com/mfa/challenge\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs:\n  - RS256\n  - PS256\n  - HS256\n  mfa:\n    supported: true\n    evidence: >-\n      mfa_challenge_endpoint and the four http://auth0.com/oauth/grant-type/mfa-* grant types are\n      advertised in the discovery document.\n  audiences_observed:\n  - https://client-portal.hli.com\n  audience_note: >-\n    Read from the Auth0 SDK configuration embedded in the portal's own main.js bundle\n    (https://portal.humanlongevity.com/main.aac5aadc52a10f4b.js). This is an OAuth audience\n    identifier for the portal's private\
  \ backend API. That backend publishes no contract and no\n    documentation, and the hli.com host that the identifier is named after does not resolve to a\n    Human Longevity property, so it is recorded as an identifier only — never as a callable base URL.\nobservations:\n- id: weak_algs_advertised\n  note: >-\n    HS256 is advertised alongside RS256/PS256 for ID token signing, and `plain` alongside S256 for\n    PKCE. Both are Auth0 tenant defaults rather than deliberate HLI choices, but a public agent\n    reading this discovery document cannot tell the difference.\n- id: no_oauth_protected_resource\n  note: >-\n    /.well-known/oauth-protected-resource returns 404, so there is no RFC 9728 resource metadata\n    pointing at a protected API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-longevity/refs/heads/main/authentication/human-longevity-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Health
- Healthcare
- Genomics
- Precision Medicine
- Diagnostics
- Artificial Intelligence
- Longevity
- Life Sciences
- Medical Imaging
---
