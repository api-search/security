---
api_key_in: []
api_specs:
- filename: reliance-jio-jiomeet-platform-openapi.yml
  format: yaml
  label: JioMeet Platform Server API
  slug: jiomeet-platform-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jiomeet-platform-openapi.yml
- filename: reliance-jio-jiomeet-oauth-openapi.yml
  format: yaml
  label: JioMeet Platform OAuth API
  slug: jiomeet-platform-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jiomeet-oauth-openapi.yml
- filename: reliance-jio-jioevents-platform-openapi.yml
  format: yaml
  label: JioEvents Platform Server API
  slug: jioevents-platform-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jioevents-platform-openapi.yml
auth_types:
- http
- jwt-bearer
- oauth2
description: 'Reliance Jio''s publicly documented authentication surface is entirely the JioMeet / JioEvents developer platform. Two distinct models are in play. Server-to-server (JioMeet Platform Server API, JioEvents Platform Server API) uses a self-signed JWT built from app credentials issued in the JioMeet console and sent in the Authorization header - the spec models it as a required header PARAMETER, not a securityScheme, so it is invisible to tooling that only reads components.securitySchemes. User-authorized access (JioMeet Platform OAuth API) is a real OAuth 2.0 authorization-code flow with HTTP Basic client authentication at the token endpoint and HTTP Bearer on every subsequent call - that surface IS modelled as securitySchemes. Jio''s network / CAMARA APIs are not in scope here: they are partner-gated through Aduna and the GSMA federated hub, and Jio publishes no CIBA endpoint and no OIDC discovery document anywhere in its estate.'
kind: authentication
layout: security
method: searched
name: Reliance Jio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Reliance Jio secures its APIs with http, jwt-bearer, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Reliance Jio
provider_slug: reliance-jio
scheme_count: 3
schemes:
- algorithms:
  - HS256
  - RS256
  applies_to:
  - openapi/reliance-jio-jiomeet-platform-openapi.yml
  - openapi/reliance-jio-jioevents-platform-openapi.yml
  credential_issuance: https://platform.jiomeet.com
  detail: One-step authentication signs the token with the app secret using HMAC SHA-256 (HS256). Two-step authentication signs with a private key using RS256 and registers the matching public key. In both cases the JWT payload must carry an issuer and an "app" claim holding the JioMeet app id generated in the platform console at https://platform.jiomeet.com. Jio's own guidance is to keep tokens short-lived and validate them server-side.
  docs: https://dev.jiomeet.com/docs/quick-start/authentication
  location: Authorization header
  modelled_as: required header parameter (not a securityScheme)
  name: jwt-app-credentials
  type: jwt
- description: OAuth clientId as the username and the OAuth client secret as the password. Used only on POST /api/oauth2/v2/token.
  name: basicAuth
  operations:
  - POST /api/oauth2/v2/token
  scheme: basic
  sources:
  - openapi/reliance-jio-jiomeet-oauth-openapi.yml
  type: http
- description: The access_token returned by /api/oauth2/v2/token, sent as an HTTP Bearer token on every user-authorized call.
  name: bearerAuth
  operation_count: 6
  scheme: bearer
  sources:
  - openapi/reliance-jio-jiomeet-oauth-openapi.yml
  type: http
slug: reliance-jio-authentication
source_filename: reliance-jio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://dev.jiomeet.com/docs/quick-start/authentication,\n  https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client, and the\n  securitySchemes / Authorization header parameters in the harvested OpenAPI\n  (openapi/reliance-jio-*-openapi.yml)\ndocs: https://dev.jiomeet.com/docs/quick-start/authentication\ndescription: >-\n  Reliance Jio's publicly documented authentication surface is entirely the JioMeet /\n  JioEvents developer platform. Two distinct models are in play. Server-to-server\n  (JioMeet Platform Server API, JioEvents Platform Server API) uses a self-signed JWT\n  built from app credentials issued in the JioMeet console and sent in the Authorization\n  header - the spec models it as a required header PARAMETER, not a securityScheme, so\n  it is invisible to tooling that only reads components.securitySchemes. User-authorized\n  access (JioMeet Platform OAuth API) is a real OAuth 2.0 authorization-code\
  \ flow with\n  HTTP Basic client authentication at the token endpoint and HTTP Bearer on every\n  subsequent call - that surface IS modelled as securitySchemes. Jio's network / CAMARA\n  APIs are not in scope here: they are partner-gated through Aduna and the GSMA\n  federated hub, and Jio publishes no CIBA endpoint and no OIDC discovery document\n  anywhere in its estate.\nsummary:\n  types: [http, jwt-bearer, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  oidc_discovery: false\n  mtls: false\n  ciba: false\nschemes:\n  - name: jwt-app-credentials\n    type: jwt\n    location: Authorization header\n    modelled_as: required header parameter (not a securityScheme)\n    algorithms: [HS256, RS256]\n    docs: https://dev.jiomeet.com/docs/quick-start/authentication\n    applies_to:\n      - openapi/reliance-jio-jiomeet-platform-openapi.yml\n      - openapi/reliance-jio-jioevents-platform-openapi.yml\n    detail: >-\n      One-step authentication signs the token with the\
  \ app secret using HMAC SHA-256\n      (HS256). Two-step authentication signs with a private key using RS256 and\n      registers the matching public key. In both cases the JWT payload must carry an\n      issuer and an \"app\" claim holding the JioMeet app id generated in the platform\n      console at https://platform.jiomeet.com. Jio's own guidance is to keep tokens\n      short-lived and validate them server-side.\n    credential_issuance: https://platform.jiomeet.com\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      OAuth clientId as the username and the OAuth client secret as the password. Used\n      only on POST /api/oauth2/v2/token.\n    sources: [openapi/reliance-jio-jiomeet-oauth-openapi.yml]\n    operations: ['POST /api/oauth2/v2/token']\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      The access_token returned by /api/oauth2/v2/token, sent as an HTTP Bearer token on\n      every user-authorized call.\n\
  \    sources: [openapi/reliance-jio-jiomeet-oauth-openapi.yml]\n    operation_count: 6\noauth2:\n  flow: authorizationCode\n  authorization_endpoint: https://jiomeetpro.jio.com/oauth2/authorize\n  token_endpoint: https://jiomeetpro.jio.com/api/oauth2/v2/token\n  token_endpoint_auth_method: client_secret_basic\n  grant_types: [authorization_code, refresh_token]\n  state_parameter: recommended (base64-encoded CSRF token)\n  scopes: scopes/reliance-jio-scopes.yml\n  token_lifetimes:\n    authorization_code: 5 minutes\n    access_token: 1 day\n    refresh_token: 60 days\n  docs: https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client\nnot_found:\n  - id: openid-connect\n    note: >-\n      No OIDC discovery document is served anywhere on a Jio host. jiomeetpro.jio.com\n      returns 403 for /.well-known/openid-configuration, dev.jiomeet.com and\n      platform.jiomeet.com return 404, and www.jio.com returns a 200 text/html SPA shell\n      for every /.well-known/ path.\n  - id:\
  \ ciba\n    note: >-\n      CIBA - the backchannel authentication mechanism CAMARA pairs with OIDC for network\n      APIs - does not appear on any Jio-operated surface, consistent with Jio publishing\n      no first-party Open Gateway portal.\n  - id: mutual-tls\n    note: No mTLS scheme is documented or declared.\n  - id: api-key\n    note: No plain apiKey scheme; app credentials are always exchanged for a JWT first.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/authentication/reliance-jio-authentication.yml
summary_line: http/jwt-bearer/oauth2 · 3 schemes
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- CPaaS
- Messaging
- Voice
- IoT
- Broadband
- 5G
- BSS
- OSS
- Standards
- Video Conferencing
---
