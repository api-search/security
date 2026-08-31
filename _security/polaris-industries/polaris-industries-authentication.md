---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Polaris Industries Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polaris Industries declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Polaris Industries
provider_slug: polaris-industries
scheme_count: 0
schemes: []
slug: polaris-industries-authentication
source_filename: polaris-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://polarisdealers.auth0.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Polaris Inc. publishes no public API and no developer portal, so there is no OpenAPI\n  securitySchemes block to derive from. What IS reachable and unauthenticated is the OpenID\n  Connect discovery document for the identity tenant that fronts the Polaris dealer portal\n  (www.polarisportal.com / www.polarisdealers.com). Everything below is read verbatim from\n  that document — nothing is inferred about the APIs it protects, because those are not\n  published. The dealer portal itself is a partner login, not an API program.\nsurfaces:\n- name: Polaris Dealer Portal identity (Auth0 tenant)\n  audience: https://polarisportal.com\n  relying_parties:\n  - https://www.polarisportal.com/\n  - https://www.polarisdealers.com/\n  issuer: https://polarisdealers.auth0.com/\n  discovery: https://polarisdealers.auth0.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  schemes:\n  - type: openIdConnect\n    openIdConnectUrl: https://polarisdealers.auth0.com/.well-known/openid-configuration\n    authorization_endpoint: https://polarisdealers.auth0.com/authorize\n    token_endpoint: https://polarisdealers.auth0.com/oauth/token\n    userinfo_endpoint: https://polarisdealers.auth0.com/userinfo\n    jwks_uri: https://polarisdealers.auth0.com/.well-known/jwks.json\n    revocation_endpoint: https://polarisdealers.auth0.com/oauth/revoke\n    registration_endpoint: https://polarisdealers.auth0.com/oidc/register\n    device_authorization_endpoint: https://polarisdealers.auth0.com/oauth/device/code\n    mfa_challenge_endpoint: https://polarisdealers.auth0.com/mfa/challenge\n    grant_types:\n    - authorization_code\n    - client_credentials\n    - refresh_token\n    - implicit\n    - password\n    - urn:ietf:params:oauth:grant-type:device_code\n    - urn:ietf:params:oauth:grant-type:token-exchange\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \    - http://auth0.com/oauth/grant-type/password-realm\n    - http://auth0.com/oauth/grant-type/passwordless/otp\n    - http://auth0.com/oauth/grant-type/mfa-oob\n    - http://auth0.com/oauth/grant-type/mfa-otp\n    - http://auth0.com/oauth/grant-type/mfa-recovery-code\n    response_types:\n    - code\n    - token\n    - id_token\n    - code token\n    - code id_token\n    - token id_token\n    - code token id_token\n    response_modes:\n    - query\n    - fragment\n    - form_post\n    pkce:\n      supported: true\n      code_challenge_methods:\n      - S256\n      - plain\n      observed_in_use: S256\n      evidence: >-\n        The live dealer-portal redirect carries code_challenge_method=S256, so the deployed\n        flow is authorization_code + PKCE, not implicit.\n    token_endpoint_auth_methods:\n    - client_secret_basic\n    - client_secret_post\n    - private_key_jwt\n    - none\n    token_endpoint_auth_signing_algs:\n    - RS256\n    - RS384\n    - PS256\n    mfa: true\n-\
  \ name: api.polaris.com\n  http_status: 500\n  schemes: []\n  note: >-\n    Live gateway host (IBM DataPower / API Connect signature x-backside-transport: FAIL FAIL\n    behind Cloudflare). Every anonymous path returns HTTP 500 with a zero-length body, so no\n    authentication scheme could be observed. Recorded as present-but-unreadable, not absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polaris-industries/refs/heads/main/authentication/polaris-industries-authentication.yml
summary_line: 0 schemes
tags:
- Fortune 1000
- Manufacturing
- Power-Sports
- Automotive
- Consumer Products
- Connected Vehicles
- Marine
---
