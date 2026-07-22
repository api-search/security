---
api_key_in: []
api_specs:
- filename: mileiq-external-openapi-original.json
  format: json
  label: MileIQ External API
  slug: mileiq-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mileiq/refs/heads/main/openapi/mileiq-external-openapi-original.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Mileiq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- implicit
overview: MileIQ secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and implicit flow(s).
provider_name: MileIQ
provider_slug: mileiq
scheme_count: 2
schemes:
- description: OAuth 2.1 Authorization Code flow. Redirect the user to the authorization endpoint with response_type=code, client_id, scope, state; exchange the returned code at the token endpoint using the client credentials; call the API with the access token as a Bearer token; refresh with the refresh token.
  flows:
  - authorizationUrl: https://oauth2.mileiq.com/oauth2/auth
    flow: authorizationCode
    refreshUrl: https://oauth2.mileiq.com/oauth2/token
    tokenUrl: https://oauth2.mileiq.com/oauth2/token
  name: OAuth2
  sources:
  - https://developer.mileiq.com/api-reference/getting-started
  type: oauth2
- description: 'Full OIDC provider. grant_types_supported: authorization_code, implicit, client_credentials, refresh_token. code_challenge_methods_supported: plain, S256. token_endpoint_auth_methods_supported: client_secret_post, client_secret_basic, private_key_jwt, none. userinfo, revocation, and front/back-channel logout endpoints.'
  endpoints:
    authorization_endpoint: https://oauth2.mileiq.com/oauth2/auth
    end_session_endpoint: https://oauth2.mileiq.com/oauth2/sessions/logout
    issuer: https://oauth2.mileiq.com/
    jwks_uri: https://oauth2.mileiq.com/.well-known/jwks.json
    revocation_endpoint: https://oauth2.mileiq.com/oauth2/revoke
    token_endpoint: https://oauth2.mileiq.com/oauth2/token
    userinfo_endpoint: https://oauth2.mileiq.com/userinfo
  name: OpenIDConnect
  openIdConnectUrl: https://oauth2.mileiq.com/.well-known/openid-configuration
  sources:
  - https://oauth2.mileiq.com/.well-known/openid-configuration
  type: openIdConnect
slug: mileiq-authentication
source_filename: mileiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.mileiq.com/api-reference/getting-started.md\ndocs: https://developer.mileiq.com/api-reference/getting-started\noidc_discovery: https://oauth2.mileiq.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, implicit]\n  token_type: Bearer\n  header: 'Authorization: Bearer <access_token>'\n  note: >-\n    The MileIQ External API OpenAPI does not declare securitySchemes; every operation\n    takes an optional Authorization header. Authentication is documented in the developer\n    portal as OAuth 2.1 (Authorization Code grant) against the oauth2.mileiq.com server,\n    with the access token sent as a Bearer token. Client ID/Secret and redirect URI are\n    issued by MileIQ on approved API-access requests.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      OAuth 2.1 Authorization\
  \ Code flow. Redirect the user to the authorization\n      endpoint with response_type=code, client_id, scope, state; exchange the returned\n      code at the token endpoint using the client credentials; call the API with the\n      access token as a Bearer token; refresh with the refresh token.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://oauth2.mileiq.com/oauth2/auth\n        tokenUrl: https://oauth2.mileiq.com/oauth2/token\n        refreshUrl: https://oauth2.mileiq.com/oauth2/token\n    sources: [https://developer.mileiq.com/api-reference/getting-started]\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://oauth2.mileiq.com/.well-known/openid-configuration\n    description: >-\n      Full OIDC provider. grant_types_supported: authorization_code, implicit,\n      client_credentials, refresh_token. code_challenge_methods_supported: plain, S256.\n      token_endpoint_auth_methods_supported: client_secret_post, client_secret_basic,\n\
  \      private_key_jwt, none. userinfo, revocation, and front/back-channel logout endpoints.\n    endpoints:\n      issuer: https://oauth2.mileiq.com/\n      authorization_endpoint: https://oauth2.mileiq.com/oauth2/auth\n      token_endpoint: https://oauth2.mileiq.com/oauth2/token\n      userinfo_endpoint: https://oauth2.mileiq.com/userinfo\n      jwks_uri: https://oauth2.mileiq.com/.well-known/jwks.json\n      revocation_endpoint: https://oauth2.mileiq.com/oauth2/revoke\n      end_session_endpoint: https://oauth2.mileiq.com/oauth2/sessions/logout\n    sources: [https://oauth2.mileiq.com/.well-known/openid-configuration]\nclient_registration: >-\n  Not self-service. A Client ID and Client Secret are issued by MileIQ per approved\n  application; request access at https://mileiq.com/en-ca/for-business/api. The API is\n  currently available on a request basis.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mileiq/refs/heads/main/authentication/mileiq-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Mileage Tracking
- Expense Management
- Transportation
- Tax
- Accounting
- Location
- Fleet
---
