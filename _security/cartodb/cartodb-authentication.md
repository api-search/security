---
api_key_in:
- header
- query
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cartodb Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: CARTO secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: CARTO
provider_slug: cartodb
scheme_count: 3
schemes:
- description: Permanent, non-expiring token generated in the CARTO Workspace. Simple to generate, scoped/restrictive, and not tied to a specific user. Passed as a Bearer token in the Authorization header (also accepted as an access_token query parameter on some map/tile endpoints).
  docs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods/api-access-tokens
  in: header
  name: API Access Token
  type: apiKey
- audience: carto-cloud-native-api
  description: Short-lived (24h) OAuth 2.0 bearer token tied to a user's permissions, obtained through the Auth0-backed CARTO identity provider. Used for both user-to-machine (SPA) and machine-to-machine access to the Cloud-Native API.
  docs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods/oauth-access-tokens
  flows:
  - authorizationUrl: https://auth.carto.com/authorize
    client_type: SPA (Single Page Application) OAuth client
    flow: authorizationCode
    grant: authorization_code
    tokenUrl: https://auth.carto.com/oauth/token
  - client_type: M2M (Machine-to-Machine) OAuth client
    flow: clientCredentials
    grant: client_credentials
    tokenUrl: https://auth.carto.com/oauth/token
  name: OAuth Access Token
  type: oauth2
- description: Auth0 OIDC discovery for the CARTO identity provider; issuer https://auth.carto.com/. Standard OIDC scopes (openid, profile, email, offline_access) supported for user login and refresh tokens.
  name: OpenID Connect
  openIdConnectUrl: https://auth.carto.com/.well-known/openid-configuration
  sources:
  - well-known/cartodb-openid-configuration.json
  type: openIdConnect
slug: cartodb-authentication
source_filename: cartodb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods\ndocs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header, query]\n  header: 'Authorization: Bearer <token>'\n  oauth2_flows: [authorizationCode, clientCredentials]\n  oauth2_audience: carto-cloud-native-api\n  identity_provider: Auth0 (auth.carto.com)\nschemes:\n- name: API Access Token\n  type: apiKey\n  in: header\n  description: >-\n    Permanent, non-expiring token generated in the CARTO Workspace. Simple to\n    generate, scoped/restrictive, and not tied to a specific user. Passed as a\n    Bearer token in the Authorization header (also accepted as an access_token\n    query parameter on some map/tile endpoints).\n  docs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods/api-access-tokens\n- name: OAuth Access\
  \ Token\n  type: oauth2\n  description: >-\n    Short-lived (24h) OAuth 2.0 bearer token tied to a user's permissions,\n    obtained through the Auth0-backed CARTO identity provider. Used for both\n    user-to-machine (SPA) and machine-to-machine access to the Cloud-Native API.\n  docs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods/oauth-access-tokens\n  audience: carto-cloud-native-api\n  flows:\n  - flow: authorizationCode\n    grant: authorization_code\n    authorizationUrl: https://auth.carto.com/authorize\n    tokenUrl: https://auth.carto.com/oauth/token\n    client_type: SPA (Single Page Application) OAuth client\n  - flow: clientCredentials\n    grant: client_credentials\n    tokenUrl: https://auth.carto.com/oauth/token\n    client_type: M2M (Machine-to-Machine) OAuth client\n- name: OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.carto.com/.well-known/openid-configuration\n  description: >-\n    Auth0 OIDC discovery for\
  \ the CARTO identity provider; issuer\n    https://auth.carto.com/. Standard OIDC scopes (openid, profile, email,\n    offline_access) supported for user login and refresh tokens.\n  sources: [well-known/cartodb-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartodb/refs/heads/main/authentication/cartodb-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Developer Tools
- Location Intelligence
- Geospatial
- Maps
- Spatial Analytics
- Data Warehouse
- GIS
- Agents
---
