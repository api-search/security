---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Npp Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- refreshToken
overview: NPP Australia (AP+) secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, deviceCode, and refreshToken flow(s).
provider_name: NPP Australia (AP+)
provider_slug: npp-australia
scheme_count: 1
schemes:
- authorizationUrl: https://auth.developers.auspayplus.com.au/authorize
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://auth.developers.auspayplus.com.au/
  jwksUri: https://auth.developers.auspayplus.com.au/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://auth.developers.auspayplus.com.au/.well-known/openid-configuration
  provider: Auth0
  scope: developer-portal login/registration (not payment-API scopes)
  scopes_supported:
  - openid
  - profile
  - offline_access
  - email
  - phone
  - address
  tokenUrl: https://auth.developers.auspayplus.com.au/oauth/token
  type: openIdConnect
slug: npp-australia-authentication
source_filename: npp-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://auth.developers.auspayplus.com.au/.well-known/openid-configuration\ndocs: https://www.developers.auspayplus.com.au/api/auth/login/\nnotes: >-\n  NPP Australia (AP+) publishes no downloadable OpenAPI, so no securitySchemes\n  could be derived. The auth model captured here is the AP+ developer-portal\n  identity layer, an Auth0 OIDC tenant on the custom domain\n  auth.developers.auspayplus.com.au. This governs registration and login to the\n  gated developer portal (NPP + BPAY + eftpos); the consumable payment APIs\n  themselves are exposed by NPP Participants under participant-specific auth and\n  their OAS3 specs sit behind portal registration.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, deviceCode, refreshToken]\n  api_key_in: []\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.developers.auspayplus.com.au/.well-known/openid-configuration\n\
  \  issuer: https://auth.developers.auspayplus.com.au/\n  authorizationUrl: https://auth.developers.auspayplus.com.au/authorize\n  tokenUrl: https://auth.developers.auspayplus.com.au/oauth/token\n  jwksUri: https://auth.developers.auspayplus.com.au/.well-known/jwks.json\n  scopes_supported: [openid, profile, offline_access, email, phone, address]\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, implicit, urn:ietf:params:oauth:grant-type:device_code, urn:ietf:params:oauth:grant-type:token-exchange]\n  provider: Auth0\n  scope: developer-portal login/registration (not payment-API scopes)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npp-australia/refs/heads/main/authentication/npp-australia-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- ISO 20022
- Payment Scheme
- Rails
- PayTo
- PayID
- Open Banking
---
