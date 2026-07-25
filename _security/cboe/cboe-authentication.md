---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Authentication profile for the Cboe LiveVol All Access API. All API access is OAuth 2.0 against the Cboe LiveVol IdentityServer at id.livevol.com, which publishes a full OpenID Connect discovery document (saved at well-known/cboe-openid-configuration.json). Machine-to-machine access uses the client_credentials grant; browser-based applications use the authorization_code flow. Access tokens are bearer tokens sent in the Authorization header and expire after 3600 seconds; refresh tokens are supported. The public Cboe Delayed Quotes JSON endpoints on cdn.cboe.com require no authentication.
kind: authentication
layout: security
method: searched
name: Cboe Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- password
- refreshToken
- implicit
overview: Cboe Global Markets secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, password, refreshToken, and implicit flow(s).
provider_name: Cboe Global Markets
provider_slug: cboe
scheme_count: 2
schemes:
- authorizationUrl: https://id.livevol.com/connect/authorize
  client_auth: Basic <base64 encoded client_id:client_secret> on the token endpoint
  grant_types_documented:
  - client_credentials
  - authorization_code
  - refresh_token
  grant_types_supported:
  - authorization_code
  - client_credentials
  - password
  - refresh_token
  - implicit
  header: 'Authorization: Bearer <access_token>'
  issuer: https://id.livevol.com
  jwksUrl: https://id.livevol.com/.well-known/jwks
  name: LiveVolOAuth2
  notes: client_credentials is documented for machine-to-machine use; authorization_code for browser-based applications. Token responses include expires_in 3600 and optional refresh_token.
  revocationUrl: https://id.livevol.com/connect/revocation
  scopes_detail: scopes/cboe-scopes.yml
  tokenUrl: https://id.livevol.com/connect/token
  type: oauth2
  userinfoUrl: https://id.livevol.com/connect/userinfo
- applies_to: https://cdn.cboe.com/api/global
  name: None (public delayed quotes)
  notes: Public delayed-quote JSON endpoints are unauthenticated.
  type: none
slug: cboe-authentication
source_filename: cboe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://api.livevol.com/v1/docs/Home/Authentication\ndocs: https://api.livevol.com/v1/docs/Home/Authentication\ndescription: >-\n  Authentication profile for the Cboe LiveVol All Access API. All API access is\n  OAuth 2.0 against the Cboe LiveVol IdentityServer at id.livevol.com, which\n  publishes a full OpenID Connect discovery document (saved at\n  well-known/cboe-openid-configuration.json). Machine-to-machine access uses\n  the client_credentials grant; browser-based applications use the\n  authorization_code flow. Access tokens are bearer tokens sent in the\n  Authorization header and expire after 3600 seconds; refresh tokens are\n  supported. The public Cboe Delayed Quotes JSON endpoints on cdn.cboe.com\n  require no authentication.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [clientCredentials, authorizationCode, password, refreshToken, implicit]\n  token_style: Bearer access token in Authorization header\n\
  \  token_lifetime_seconds: 3600\nschemes:\n  - name: LiveVolOAuth2\n    type: oauth2\n    issuer: https://id.livevol.com\n    authorizationUrl: https://id.livevol.com/connect/authorize\n    tokenUrl: https://id.livevol.com/connect/token\n    revocationUrl: https://id.livevol.com/connect/revocation\n    userinfoUrl: https://id.livevol.com/connect/userinfo\n    jwksUrl: https://id.livevol.com/.well-known/jwks\n    grant_types_documented: [client_credentials, authorization_code, refresh_token]\n    grant_types_supported: [authorization_code, client_credentials, password, refresh_token, implicit]\n    client_auth: 'Basic <base64 encoded client_id:client_secret> on the token endpoint'\n    header: 'Authorization: Bearer <access_token>'\n    scopes_detail: scopes/cboe-scopes.yml\n    notes: >-\n      client_credentials is documented for machine-to-machine use;\n      authorization_code for browser-based applications. Token responses\n      include expires_in 3600 and optional refresh_token.\n\
  \  - name: None (public delayed quotes)\n    type: none\n    applies_to: https://cdn.cboe.com/api/global\n    notes: Public delayed-quote JSON endpoints are unauthenticated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cboe/refs/heads/main/authentication/cboe-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Market Data
- Options
- Equities
- Derivatives
- Volatility
- Financial Markets
- Exchanges
- Trading
---
