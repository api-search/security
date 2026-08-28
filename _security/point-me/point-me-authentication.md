---
api_key_in: []
auth_types: []
description: How a caller authenticates to point.me. Identity is an Auth0 tenant at auth.point.me exposing a complete OIDC discovery document; the API host api.point.me is a bearer-token resource server that refuses every anonymous request. No public API credential issuance exists — access to api.point.me is arranged through the Gateway partnership sales process.
kind: authentication
layout: security
method: probed
name: Point Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: POINT.ME declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: POINT.ME
provider_slug: point-me
scheme_count: 0
schemes: []
slug: point-me-authentication
source_filename: point-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://auth.point.me/.well-known/openid-configuration (HTTP 200, fetched 2026-08-26)\n  for the identity layer, and the live response headers of https://api.point.me/\n  (HTTP 401, WWW-Authenticate: Bearer) for the API layer. point.me publishes no\n  developer authentication page; everything here is read off surfaces it actually serves.\ndescription: >-\n  How a caller authenticates to point.me. Identity is an Auth0 tenant at\n  auth.point.me exposing a complete OIDC discovery document; the API host\n  api.point.me is a bearer-token resource server that refuses every anonymous\n  request. No public API credential issuance exists — access to api.point.me is\n  arranged through the Gateway partnership sales process.\napi: point-me-flight-search-api\nbase_url: https://api.point.me\n\nsecurity_schemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n\
  \    evidence: >-\n      https://api.point.me/ and every other probed path return\n      `www-authenticate: Bearer`. The token issuer is the auth.point.me Auth0\n      tenant, whose id_token signing algs are HS256/RS256/PS256.\n    method: probed\n  - name: oidc\n    type: openIdConnect\n    openid_connect_url: https://auth.point.me/.well-known/openid-configuration\n    issuer: https://auth.point.me/\n    authorization_endpoint: https://auth.point.me/authorize\n    token_endpoint: https://auth.point.me/oauth/token\n    userinfo_endpoint: https://auth.point.me/userinfo\n    jwks_uri: https://auth.point.me/.well-known/jwks.json\n    registration_endpoint: https://auth.point.me/oidc/register\n    revocation_endpoint: https://auth.point.me/oauth/revoke\n    end_session_endpoint: https://auth.point.me/oidc/logout\n    device_authorization_endpoint: https://auth.point.me/oauth/device/code\n    method: probed\n\noauth2:\n  provider: Auth0\n  grant_types:\n    - authorization_code\n    - client_credentials\n\
  \    - refresh_token\n    - password\n    - implicit\n    - urn:ietf:params:oauth:grant-type:device_code\n    - urn:ietf:params:oauth:grant-type:token-exchange\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n    - http://auth0.com/oauth/grant-type/password-realm\n    - http://auth0.com/oauth/grant-type/passwordless/otp\n    - http://auth0.com/oauth/grant-type/mfa-oob\n    - http://auth0.com/oauth/grant-type/mfa-otp\n    - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  pkce:\n    supported: true\n    code_challenge_methods: [S256, plain]\n  id_token_signing_algs: [HS256, RS256, PS256]\n  dynamic_client_registration: true\n  mfa:\n    supported: true\n    evidence: >-\n      mfa_challenge_endpoint https://auth.point.me/mfa/challenge plus the\n      mfa-oob / mfa-otp / mfa-recovery-code\
  \ grant types in the discovery document.\n  notes: >-\n    These are the capabilities the Auth0 tenant advertises, not necessarily the\n    subset point.me enables for any given client. `client_credentials` being\n    present is the machine-to-machine path a Gateway partner would most likely use.\n\nsso:\n  supported: true\n  evidence: >-\n    \"SSO integration\" is listed under Enterprise-Grade Security on\n    https://www.point.me/partnerships/financial-institutions/ — a Gateway\n    partner capability, not a self-service one.\n\ncredential_issuance:\n  self_service: false\n  detail: >-\n    There is no developer signup, key page, or console for api.point.me. The only\n    published route to credentials is the \"Book a demo\" HubSpot form on the Gateway\n    partnership pages.\n  docs: https://www.point.me/partnerships/\n\nx-evidence:\n  checked: '2026-08-26'\n  probes:\n    - url: https://auth.point.me/.well-known/openid-configuration\n      status: 200\n    - url: https://auth.point.me/.well-known/jwks.json\n\
  \      status: 200\n    - url: https://api.point.me/\n      status: 200\n      note: 'body \"Flight Search APIs\"; every deeper path answers 401 Bearer'\n    - url: https://api.point.me/docs\n      status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/point-me/refs/heads/main/authentication/point-me-authentication.yml
summary_line: 0 schemes
tags:
- Travel
- Award Travel
- Loyalty
- Points and Miles
- Flights
- Rewards
- Embedded Finance
- Banking
- Search
- Company
---
