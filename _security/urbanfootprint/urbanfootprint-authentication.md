---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Urbanfootprint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- implicit
- password
- tokenExchange
overview: UrbanFootprint secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, implicit, password, and tokenExchange flow(s).
provider_name: UrbanFootprint
provider_slug: urbanfootprint
scheme_count: 2
schemes:
- authorizationUrl: https://login.urbanfootprint.com/authorize
  deviceAuthorizationUrl: https://login.urbanfootprint.com/oauth/device/code
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://login.urbanfootprint.com/
  jwksUri: https://login.urbanfootprint.com/.well-known/jwks.json
  name: auth0-oidc
  openIdConnectUrl: https://login.urbanfootprint.com/.well-known/openid-configuration
  provider: Auth0 (custom domain)
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  tokenUrl: https://login.urbanfootprint.com/oauth/token
  type: openIdConnect
- description: The platform API (https://app-api.urbanfootprint.com) requires an authenticated session; unauthenticated requests receive an RFC 9457 401 problem ("User must be logged in to perform this action") with access-control-allow-origin locked to https://app.urbanfootprint.com.
  name: platform-session
  type: http
slug: urbanfootprint-authentication
source_filename: urbanfootprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://login.urbanfootprint.com/.well-known/openid-configuration\nnotes: UrbanFootprint publishes no public developer API or API-key program. The\n  platform (app.urbanfootprint.com) authenticates users through an Auth0 custom\n  domain (login.urbanfootprint.com, tenant urbanfootprint) and the SPA calls the\n  platform API at app-api.urbanfootprint.com with session credentials.\n  This profile describes that live platform auth surface, not a public API contract.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, deviceCode,\n    implicit, password, tokenExchange]\n  pkce: [S256, plain]\n  dpop_signing_algs: [ES256]\nschemes:\n- name: auth0-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://login.urbanfootprint.com/.well-known/openid-configuration\n  issuer: https://login.urbanfootprint.com/\n  authorizationUrl: https://login.urbanfootprint.com/authorize\n\
  \  tokenUrl: https://login.urbanfootprint.com/oauth/token\n  deviceAuthorizationUrl: https://login.urbanfootprint.com/oauth/device/code\n  jwksUri: https://login.urbanfootprint.com/.well-known/jwks.json\n  scopes_supported: [openid, profile, offline_access, name, given_name,\n    family_name, nickname, email, email_verified, picture, created_at,\n    identities, phone, address]\n  id_token_signing_algs: [HS256, RS256, PS256]\n  provider: Auth0 (custom domain)\n- name: platform-session\n  type: http\n  description: The platform API (https://app-api.urbanfootprint.com) requires an\n    authenticated session; unauthenticated requests receive an RFC 9457 401\n    problem (\"User must be logged in to perform this action\") with\n    access-control-allow-origin locked to https://app.urbanfootprint.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanfootprint/refs/heads/main/authentication/urbanfootprint-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Climate
- Geospatial
- Urban Planning
- Data
- Analytics
- Resilience
- Mapping
---
