---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 360 Privacy Authentication
name_suffix: Authentication
oauth_flows: []
overview: 360 Privacy declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 360 Privacy
provider_slug: 360-privacy
scheme_count: 3
schemes:
- description: OpenID Connect sign-in for the 360 Privacy customer dashboard and the gated GitBook documentation. Universal Login is served at /u/login/identifier.
  id: oidc_customer_dashboard
  openIdConnectUrl: https://auth.360privacy.io/.well-known/openid-configuration
  type: openIdConnect
- authorizationUrl: https://auth.360privacy.io/authorize
  description: Authorization Code with PKCE (S256 and plain advertised).
  flow: authorizationCode
  id: oauth2_authorization_code
  pkce: true
  tokenUrl: https://auth.360privacy.io/oauth/token
  type: oauth2
- description: client_credentials is advertised in grant_types_supported by the tenant. This is the Auth0 default advertisement and is NOT documented by 360 Privacy as a machine-to-machine API surface; no audience, no protected resource and no API reference is published.
  flow: clientCredentials
  id: oauth2_client_credentials
  tokenUrl: https://auth.360privacy.io/oauth/token
  type: oauth2
slug: 360-privacy-authentication
source_filename: 360-privacy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://auth.360privacy.io/.well-known/openid-configuration\nscope_note: >-\n  IMPORTANT — what this profile does and does not cover. 360 Privacy publishes no public API and\n  no API reference, so there is no API authentication model to document. What IS published, and\n  what is captured here, is a standards-compliant OpenID Connect Discovery document served from\n  the company's own Auth0 custom domain. It governs sign-in to the authenticated customer\n  dashboard and to the Auth0-gated GitBook documentation at docs.360privacy.io. Do not read this\n  artifact as evidence of a developer-facing authentication surface.\nprovider: Auth0 (custom domain auth.360privacy.io, CNAME to CloudFront)\nissuer: https://auth.360privacy.io/\ndiscovery:\n  openid_configuration: https://auth.360privacy.io/.well-known/openid-configuration\n  oauth_authorization_server: https://auth.360privacy.io/.well-known/oauth-authorization-server\n  jwks_uri:\
  \ https://auth.360privacy.io/.well-known/jwks.json\n  http_status: 200\nendpoints:\n  authorization: https://auth.360privacy.io/authorize\n  token: https://auth.360privacy.io/oauth/token\n  userinfo: https://auth.360privacy.io/userinfo\n  revocation: https://auth.360privacy.io/oauth/revoke\n  registration: https://auth.360privacy.io/oidc/register\n  device_authorization: https://auth.360privacy.io/oauth/device/code\n  backchannel_authentication: https://auth.360privacy.io/bc-authorize\n  mfa_challenge: https://auth.360privacy.io/mfa/challenge\nschemes:\n- id: oidc_customer_dashboard\n  type: openIdConnect\n  openIdConnectUrl: https://auth.360privacy.io/.well-known/openid-configuration\n  description: >-\n    OpenID Connect sign-in for the 360 Privacy customer dashboard and the gated GitBook\n    documentation. Universal Login is served at /u/login/identifier.\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://auth.360privacy.io/authorize\n\
  \  tokenUrl: https://auth.360privacy.io/oauth/token\n  pkce: true\n  description: Authorization Code with PKCE (S256 and plain advertised).\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.360privacy.io/oauth/token\n  description: >-\n    client_credentials is advertised in grant_types_supported by the tenant. This is the Auth0\n    default advertisement and is NOT documented by 360 Privacy as a machine-to-machine API\n    surface; no audience, no protected resource and no API reference is published.\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- 'urn:ietf:params:oauth:grant-type:device_code'\n- 'urn:ietf:params:oauth:grant-type:token-exchange'\n- 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n- 'http://auth0.com/oauth/grant-type/password-realm'\n- 'http://auth0.com/oauth/grant-type/passwordless/otp'\n- 'http://auth0.com/oauth/grant-type/mfa-oob'\n- 'http://auth0.com/oauth/grant-type/mfa-otp'\n\
  - 'http://auth0.com/oauth/grant-type/mfa-recovery-code'\nscopes_supported:\n- openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\nscopes_note: >-\n  These are the stock OIDC/Auth0 identity scopes advertised by the tenant. There is no API\n  permission or authorization scope surface, which is why no scopes/ artifact is written for\n  this provider.\ntoken_signing:\n  id_token_algs: [HS256, RS256, PS256]\n  jwks_keys: 2\n  jwks_algs: [RS256, RS256]\n  dpop_signing_algs: [ES256]\nmfa:\n  supported: true\n  evidence: mfa_challenge_endpoint plus mfa-oob / mfa-otp / mfa-recovery-code grant types\nfeatures:\n  pkce: true\n  dpop: true\n  backchannel_logout: true\n  dynamic_client_registration: true\n  global_token_revocation: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/360-privacy/refs/heads/main/authentication/360-privacy-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Privacy
- Data Removal
- Executive Protection
- Cybersecurity
- Threat Intelligence
- Dark Web Monitoring
- Personal Data
- Managed Services
---
