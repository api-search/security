---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Mutual Of America Life Insurance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mutual of America Life Insurance Company declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mutual of America Life Insurance Company
provider_slug: mutual-of-america-life-insurance
scheme_count: 2
schemes:
- description: OpenID Connect Discovery 1.0. Sign-in for employees, individuals and plan sponsors reaching the retirement plan portal.
  issuer: https://login.mutualofamerica.com
  key: openIdConnect
  openIdConnectUrl: https://login.mutualofamerica.com/.well-known/openid-configuration
  type: openIdConnect
- description: RFC 8414 OAuth 2.0 Authorization Server Metadata for the same issuer.
  flows:
    authorizationCode:
      authorizationUrl: https://login.mutualofamerica.com/oauth2/v1/authorize
      refreshUrl: https://login.mutualofamerica.com/oauth2/v1/token
      tokenUrl: https://login.mutualofamerica.com/oauth2/v1/token
    clientCredentials:
      note: client_credentials is advertised by the OAuth 2.0 authorization-server metadata only, not by the OpenID Connect document.
      tokenUrl: https://login.mutualofamerica.com/oauth2/v1/token
    implicit:
      authorizationUrl: https://login.mutualofamerica.com/oauth2/v1/authorize
      note: Advertised but legacy; authorization code with PKCE is the modern path.
  key: oauth2
  metadata: https://login.mutualofamerica.com/.well-known/oauth-authorization-server
  type: oauth2
slug: mutual-of-america-life-insurance-authentication
source_filename: mutual-of-america-life-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://login.mutualofamerica.com/.well-known/openid-configuration\nscope_of_this_artifact: >-\n  This describes the ONLY authorization surface Mutual of America publishes machine-readable\n  metadata for: the customer/plan-participant identity host at login.mutualofamerica.com. It is\n  NOT a public API authentication profile — Mutual of America publishes no developer program,\n  no API reference and no OpenAPI, so there are no securitySchemes to derive from a contract.\n  Everything below was read directly from the two discovery documents saved under well-known/.\nprovider_hosts:\n  - host: login.mutualofamerica.com\n    platform: Okta Customer Identity (custom domain; issuer matches the host)\n    verified: probed\nschemes:\n  - key: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://login.mutualofamerica.com/.well-known/openid-configuration\n    issuer: https://login.mutualofamerica.com\n    description:\
  \ >-\n      OpenID Connect Discovery 1.0. Sign-in for employees, individuals and plan sponsors\n      reaching the retirement plan portal.\n  - key: oauth2\n    type: oauth2\n    metadata: https://login.mutualofamerica.com/.well-known/oauth-authorization-server\n    description: RFC 8414 OAuth 2.0 Authorization Server Metadata for the same issuer.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://login.mutualofamerica.com/oauth2/v1/authorize\n        tokenUrl: https://login.mutualofamerica.com/oauth2/v1/token\n        refreshUrl: https://login.mutualofamerica.com/oauth2/v1/token\n      clientCredentials:\n        tokenUrl: https://login.mutualofamerica.com/oauth2/v1/token\n        note: >-\n          client_credentials is advertised by the OAuth 2.0 authorization-server metadata only,\n          not by the OpenID Connect document.\n      implicit:\n        authorizationUrl: https://login.mutualofamerica.com/oauth2/v1/authorize\n        note: Advertised but legacy;\
  \ authorization code with PKCE is the modern path.\nendpoints:\n  authorization: https://login.mutualofamerica.com/oauth2/v1/authorize\n  token: https://login.mutualofamerica.com/oauth2/v1/token\n  userinfo: https://login.mutualofamerica.com/oauth2/v1/userinfo\n  jwks: https://login.mutualofamerica.com/oauth2/v1/keys\n  introspection: https://login.mutualofamerica.com/oauth2/v1/introspect\n  revocation: https://login.mutualofamerica.com/oauth2/v1/revoke\n  end_session: https://login.mutualofamerica.com/oauth2/v1/logout\n  device_authorization: https://login.mutualofamerica.com/oauth2/v1/device/authorize\n  pushed_authorization_request: https://login.mutualofamerica.com/oauth2/v1/par\n  dynamic_client_registration: https://login.mutualofamerica.com/oauth2/v1/clients\ngrant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:openid:params:grant-type:ciba'\nclient_authentication_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\ntoken_security:\n  pkce: true\n  code_challenge_methods: [S256]\n  par_supported: true\n  dpop_supported: true\n  dpop_signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512]\n  id_token_signing_algs: [RS256]\n  id_token_encryption_algs: [RSA-OAEP-256, RSA-OAEP-384, RSA-OAEP-512]\n  request_object_supported: true\n  mtls_supported: false\n  note: >-\n    PKCE is advertised with S256 only (no `plain`), pushed authorization requests are\n    supported, and DPoP sender-constrained tokens are available — a modern posture for the\n    sign-in surface. The `password` and `implicit` grants remain advertised, which is the one\n    weak signal here.\napi_keys: none-published\nmutual_tls: not-advertised\ndocs: null\ndocs_note: >-\n  Mutual of America publishes no developer authentication documentation. Probed and confirmed\n  absent on 2026-08-28: www.mutualofamerica.com returns HTTP 404 for\
  \ /openapi.json,\n  /swagger.json, /api-docs, /docs, /graphql and /llms.txt, and developer., api. and\n  docs.mutualofamerica.com do not resolve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutual-of-america-life-insurance/refs/heads/main/authentication/mutual-of-america-life-insurance-authentication.yml
summary_line: 2 schemes
tags:
- Insurance
- Life Insurance
- Retirement
- Financial Services
- Pensions
- Annuities
- Wealth Management
- Identity
---
