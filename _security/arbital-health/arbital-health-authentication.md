---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Arbital Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Arbital Health secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Arbital Health
provider_slug: arbital-health
scheme_count: 1
schemes:
- claims_supported:
  - email
  - email_verified
  - exp
  - first_name
  - last_name
  - iat
  - iss
  - picture_url
  code_challenge_methods_supported:
  - S256
  endpoints:
    authorization: https://auth.arbitalhealth.com/propelauth/oauth/authorize
    jwks: https://auth.arbitalhealth.com/.well-known/jwks.json
    token: https://auth.arbitalhealth.com/propelauth/oauth/token
    userinfo: https://auth.arbitalhealth.com/propelauth/oauth/userinfo
  grant_types_supported:
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://auth.arbitalhealth.com
  name: propelauth-oidc
  openIdConnectUrl: https://auth.arbitalhealth.com/.well-known/openid-configuration
  provider: PropelAuth
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - profile
  sources:
  - well-known/arbital-health-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: arbital-health-authentication
source_filename: arbital-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.arbitalhealth.com/.well-known/openid-configuration\ndocs: null\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Derived from the live OpenID Connect discovery document, not from an OpenAPI —\n    Arbital Health publishes no machine-readable API contract. The platform API at\n    platform.arbitalhealth.com/api returns 401 {\"error\":\"Unauthorized\"} to every\n    anonymous request, so the credential material it accepts (bearer JWT vs session\n    cookie) could not be confirmed without a customer account.\nschemes:\n- name: propelauth-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.arbitalhealth.com/.well-known/openid-configuration\n  issuer: https://auth.arbitalhealth.com\n  provider: PropelAuth\n  sources:\n  - well-known/arbital-health-openid-configuration.json\n  endpoints:\n    authorization: https://auth.arbitalhealth.com/propelauth/oauth/authorize\n\
  \    token: https://auth.arbitalhealth.com/propelauth/oauth/token\n    userinfo: https://auth.arbitalhealth.com/propelauth/oauth/userinfo\n    jwks: https://auth.arbitalhealth.com/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  claims_supported:\n  - email\n  - email_verified\n  - exp\n  - first_name\n  - last_name\n  - iat\n  - iss\n  - picture_url\nobservations:\n- Authorization Code + PKCE (S256) is the only advertised flow; no client_credentials,\n  no device flow, no refresh_token grant advertised.\n- No /.well-known/oauth-authorization-server (RFC 8414) and no\n  /.well-known/oauth-protected-resource (RFC 9728) are published — both\
  \ 404.\n- Single-tenant SaaS login. There is no public developer registration path; OAuth\n  clients are provisioned by Arbital Health for its customers.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://auth.arbitalhealth.com/.well-known/openid-configuration\n    status: 200\n  - url: https://auth.arbitalhealth.com/.well-known/jwks.json\n    status: 200\n  - url: https://platform.arbitalhealth.com/api/v1\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbital-health/refs/heads/main/authentication/arbital-health-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Health Insurance
- Value-Based Care
- Actuarial
- Claims
- Payers
- Providers
- Analytics
- Artificial Intelligence
---
