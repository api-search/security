---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: World Fuel Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: World Fuel Services declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: World Fuel Services
provider_slug: world-fuel-services
scheme_count: 1
schemes:
- dpop_signing_algs:
  - ES256
  endpoints:
    authorization: https://auth.wfscorp.com/authorize
    backchannel_authentication: https://auth.wfscorp.com/bc-authorize
    device_authorization: https://auth.wfscorp.com/oauth/device/code
    dynamic_registration: https://auth.wfscorp.com/oidc/register
    jwks: https://auth.wfscorp.com/.well-known/jwks.json
    mfa_challenge: https://auth.wfscorp.com/mfa/challenge
    revocation: https://auth.wfscorp.com/oauth/revoke
    token: https://auth.wfscorp.com/oauth/token
    userinfo: https://auth.wfscorp.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: openid-connect
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.wfscorp.com/
  logout:
    backchannel_logout_session_supported: true
    backchannel_logout_supported: true
  mfa:
    evidence: mfa_challenge_endpoint and the mfa-oob / mfa-otp / mfa-recovery-code grant types.
    supported: true
  observations:
  - The `implicit` and `password` (ROPC) grants are still advertised alongside authorization_code + PKCE; both are discouraged by OAuth 2.1.
  - '`plain` remains in code_challenge_methods_supported next to S256.'
  - HS256 is advertised for id_token signing alongside RS256/PS256.
  - No custom API scopes appear in scopes_supported — only the OIDC/profile set.
  openIdConnectUrl: https://auth.wfscorp.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  platform: Auth0 (custom domain)
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: world-fuel-services-authentication
source_filename: world-fuel-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://auth.wfscorp.com/.well-known/openid-configuration\nnote: >-\n  World Kinect publishes no public developer program and no OpenAPI, so there are no\n  securitySchemes to derive from. What it DOES publish anonymously is a full OpenID Connect\n  Discovery document on auth.wfscorp.com — the Auth0-backed identity host that the myWorld\n  customer portal (myworld.wfscorp.com) authenticates against. Everything below is read\n  verbatim from that document; nothing is inferred. Access to the APIs the portal calls is\n  still gated: the tenant issues tokens only to registered clients, and a customer requests\n  portal access through a sales form rather than self-service signup.\ndomain_ownership: >-\n  wfscorp.com is World Kinect Corporation's own legacy corporate domain — it 301s to\n  www.world-kinect.com and the myWorld portal SPA served from myworld.wfscorp.com names\n  auth.wfscorp.com as its issuer in its published JavaScript\
  \ bundle.\nschemes:\n- id: openid-connect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.wfscorp.com/.well-known/openid-configuration\n  issuer: https://auth.wfscorp.com/\n  platform: Auth0 (custom domain)\n  endpoints:\n    authorization: https://auth.wfscorp.com/authorize\n    token: https://auth.wfscorp.com/oauth/token\n    userinfo: https://auth.wfscorp.com/userinfo\n    jwks: https://auth.wfscorp.com/.well-known/jwks.json\n    revocation: https://auth.wfscorp.com/oauth/revoke\n    device_authorization: https://auth.wfscorp.com/oauth/device/code\n    backchannel_authentication: https://auth.wfscorp.com/bc-authorize\n    dynamic_registration: https://auth.wfscorp.com/oidc/register\n    mfa_challenge: https://auth.wfscorp.com/mfa/challenge\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_algs:\n  - ES256\n  mfa:\n    supported: true\n    evidence: mfa_challenge_endpoint and the mfa-oob / mfa-otp / mfa-recovery-code grant types.\n  logout:\n    backchannel_logout_supported: true\n    backchannel_logout_session_supported: true\n  observations:\n  - The `implicit` and `password` (ROPC) grants are still advertised alongside\n    authorization_code + PKCE; both are discouraged by OAuth 2.1.\n  - '`plain` remains in code_challenge_methods_supported next to S256.'\n  - HS256 is advertised for id_token signing alongside RS256/PS256.\n  - No custom API scopes appear in scopes_supported\
  \ — only the OIDC/profile set.\nonboarding:\n  self_service: false\n  path: https://www.world-kinect.com/about-us/contact-us/portal-access-form\n  note: >-\n    Portal access is requested through a form; there is no public API key issuance, no\n    documented client-credentials onboarding, and no published developer terms.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-fuel-services/refs/heads/main/authentication/world-fuel-services-authentication.yml
summary_line: 1 scheme
tags:
- Fortune 100
- Energy
- Aviation Fuel
- Marine Fuel
- Fuel Distribution
- Energy Management
- Sustainability
- Logistics
- Fuel Cards
---
