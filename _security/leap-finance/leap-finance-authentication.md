---
api_key_in: []
auth_types: []
description: Authentication profile for Leap Finance Inc., established entirely by probing the company's own identity tenant. Leap Finance publishes no API reference and no OpenAPI document, so there are no securitySchemes to derive from. What it does serve is a complete, unauthenticated OpenID Connect discovery document at auth.leapfinance.com — an Auth0 tenant on the company's own domain — which describes the identity surface behind its consumer loan application and partner portal.
kind: authentication
layout: security
method: probed
name: Leap Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leap Finance declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Leap Finance
provider_slug: leap-finance
scheme_count: 2
schemes:
- description: OpenID Connect 1.0, discovered live. Also served, byte-identical, at the RFC 8414 path /.well-known/oauth-authorization-server.
  id: openIdConnect
  openIdConnectUrl: https://auth.leapfinance.com/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth 2.0 authorization server fronting the same tenant.
  flows:
    authorizationCode:
      authorizationUrl: https://auth.leapfinance.com/authorize
      refreshUrl: https://auth.leapfinance.com/oauth/token
      tokenUrl: https://auth.leapfinance.com/oauth/token
    clientCredentials:
      tokenUrl: https://auth.leapfinance.com/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://auth.leapfinance.com/oauth/device/code
      tokenUrl: https://auth.leapfinance.com/oauth/token
    implicit:
      authorizationUrl: https://auth.leapfinance.com/authorize
      note: Advertised but deprecated by OAuth 2.1; listed here because the tenant declares it, not because it is recommended.
  id: oauth2
  type: oauth2
slug: leap-finance-authentication
source_filename: leap-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  https://auth.leapfinance.com/.well-known/openid-configuration (HTTP 200,\n  application/json, 2523 bytes, fetched 2026-08-25) — saved verbatim to\n  well-known/leap-finance-openid-configuration.json\nname: Leap Finance authentication\ndescription: >-\n  Authentication profile for Leap Finance Inc., established entirely by probing the\n  company's own identity tenant. Leap Finance publishes no API reference and no\n  OpenAPI document, so there are no securitySchemes to derive from. What it does\n  serve is a complete, unauthenticated OpenID Connect discovery document at\n  auth.leapfinance.com — an Auth0 tenant on the company's own domain — which\n  describes the identity surface behind its consumer loan application and partner\n  portal.\n\ncaveat: >-\n  This describes an END-USER IDENTITY surface, not a developer API authentication\n  model. The endpoints below authenticate borrowers and partner-portal operators into\n\
  \  Leap Finance's own web applications. No public API accepts these tokens, because no\n  public API is documented. Do not read this artifact as evidence that Leap Finance\n  offers programmatic access.\n\nprovider: Auth0\nissuer: https://auth.leapfinance.com/\ntenant_cname: auth-leapfinance-cd-gp8aezmavuzbqnge.edge.tenants.auth0.com\n\nschemes:\n  - id: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://auth.leapfinance.com/.well-known/openid-configuration\n    description: >-\n      OpenID Connect 1.0, discovered live. Also served, byte-identical, at the RFC\n      8414 path /.well-known/oauth-authorization-server.\n  - id: oauth2\n    type: oauth2\n    description: OAuth 2.0 authorization server fronting the same tenant.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://auth.leapfinance.com/authorize\n        tokenUrl: https://auth.leapfinance.com/oauth/token\n        refreshUrl: https://auth.leapfinance.com/oauth/token\n      clientCredentials:\n\
  \        tokenUrl: https://auth.leapfinance.com/oauth/token\n      deviceCode:\n        deviceAuthorizationUrl: https://auth.leapfinance.com/oauth/device/code\n        tokenUrl: https://auth.leapfinance.com/oauth/token\n      implicit:\n        authorizationUrl: https://auth.leapfinance.com/authorize\n        note: >-\n          Advertised but deprecated by OAuth 2.1; listed here because the tenant\n          declares it, not because it is recommended.\n\nendpoints:\n  authorization: https://auth.leapfinance.com/authorize\n  token: https://auth.leapfinance.com/oauth/token\n  userinfo: https://auth.leapfinance.com/userinfo\n  jwks: https://auth.leapfinance.com/.well-known/jwks.json\n  revocation: https://auth.leapfinance.com/oauth/revoke\n  registration: https://auth.leapfinance.com/oidc/register\n  device_authorization: https://auth.leapfinance.com/oauth/device/code\n  backchannel_authentication: https://auth.leapfinance.com/bc-authorize\n  mfa_challenge: https://auth.leapfinance.com/mfa/challenge\n\
  \  global_token_revocation: https://auth.leapfinance.com/oauth/global-token-revocation/connection/{connectionName}\n\ngrant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n\nclient_authentication:\n  token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    - private_key_jwt\n    - none\n  token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, PS256]\n\ntoken_security:\n  pkce:\n    supported: true\n    code_challenge_methods_supported: [S256, plain]\n    note: >-\n  \
  \    S256 is supported. `plain` is also advertised, which RFC 7636 permits but\n      discourages for clients capable of S256.\n  dpop:\n    supported: true\n    dpop_signing_alg_values_supported: [ES256]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  note: >-\n    HS256 is advertised for ID token signing alongside RS256/PS256. HS256 is a\n    symmetric algorithm and is only appropriate for confidential clients.\n\nmfa:\n  supported: true\n  evidence: >-\n    mfa_challenge_endpoint plus the mfa-oob / mfa-otp / mfa-recovery-code grant types\n    in the discovery document.\n\nregistration:\n  dynamic_client_registration: true\n  endpoint: https://auth.leapfinance.com/oidc/register\n  note: >-\n    RFC 7591 dynamic client registration endpoint is advertised. Whether it is open\n    or requires an initial access token was NOT tested — this pipeline does not\n    attempt registration against a live identity tenant.\n\nsubject_types_supported: [public]\nresponse_modes_supported:\
  \ [query, fragment, form_post]\nresponse_types_supported:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n\nrequest_object:\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\n\nclaims_supported:\n  - aud\n  - auth_time\n  - created_at\n  - email\n  - email_verified\n  - exp\n  - family_name\n  - given_name\n  - iat\n  - identities\n  - iss\n  - name\n  - nickname\n  - phone_number\n  - picture\n  - sub\n\nscopes:\n  reference: scopes/leap-finance-scopes.yml\n\nother_hosts:\n  - host: api.leapscholar.com\n    observed: >-\n      Rejects all unauthenticated requests. Returns HTTP 403 with an empty body on\n      /, /v1/* and every /.well-known/* path, and HTTP 400 application/problem+json\n      on other paths. No WWW-Authenticate header is returned, so the expected\n      credential type is not advertised. Authentication model undetermined.\n  - host: partner.leapfinance.com\n    observed:\
  \ >-\n      React single-page application titled \"Leap Finance\" that renders nothing\n      without JavaScript. A partner portal login; no machine-readable auth metadata.\n  - host: portal.leapfinance.com\n    observed: >-\n      Next.js application whose served body is \"Home Visit CMS Login\" — an internal\n      operations CMS. Not a developer surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leap-finance/refs/heads/main/authentication/leap-finance-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Financial Services
- Lending
- Student Loans
- Education Finance
- Fintech
- Consumer Finance
- Study Abroad
- India
---
