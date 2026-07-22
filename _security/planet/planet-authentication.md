---
api_key_in:
- header
- query
- basic-auth-username
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Planet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: Planet secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: Planet
provider_slug: planet
scheme_count: 3
schemes:
- description: 'Planet API key. Presented three ways - (1) HTTP Basic auth with the API key as the username and an empty password (preferred where supported); (2) an Authorization header of the form `Authorization: api-key <api_key>`; (3) an `api_key` URL query parameter. Keys are found on the Account page under My Settings.'
  in:
  - header
  - query
  locations:
    basic_auth: username=<api_key>, password empty
    header: 'Authorization: api-key <api_key>'
    query: api_key=<api_key>
  name: PlanetAPIKey
  type: apiKey
- description: 'OAuth2 / OIDC via login.planet.com (Auth0-backed). Authorization Code grant for interactive user sessions (supports MFA and federated login); Client Credentials grant for machine-to-machine (rolling out for api.planet.com, available today for Sentinel Hub services). Access tokens are JWTs presented as `Authorization: Bearer <access_token>`.'
  flows:
  - authorizationUrl: https://login.planet.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.planet.com/oauth/token
  - flow: clientCredentials
    note: Machine-to-machine; for Sentinel Hub services the token endpoint is https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token
    tokenUrl: https://login.planet.com/oauth/token
  - deviceAuthorizationUrl: https://login.planet.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://login.planet.com/oauth/token
  name: PlanetOAuth2
  type: oauth2
- description: OpenID Connect discovery is published at login.planet.com. Issuer https://login.planet.com/, JWKS at /.well-known/jwks.json.
  name: PlanetOIDC
  openIdConnectUrl: https://login.planet.com/.well-known/openid-configuration
  type: openIdConnect
slug: planet-authentication
source_filename: planet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.planet.com/develop/authentication/\ndocs: https://docs.planet.com/develop/authentication/\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header, query, basic-auth-username]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode]\nschemes:\n- name: PlanetAPIKey\n  type: apiKey\n  description: >-\n    Planet API key. Presented three ways - (1) HTTP Basic auth with the API key as\n    the username and an empty password (preferred where supported); (2) an\n    Authorization header of the form `Authorization: api-key <api_key>`; (3) an\n    `api_key` URL query parameter. Keys are found on the Account page under My\n    Settings.\n  in: [header, query]\n  locations:\n    basic_auth: username=<api_key>, password empty\n    header: 'Authorization: api-key <api_key>'\n    query: api_key=<api_key>\n- name: PlanetOAuth2\n  type: oauth2\n  description: >-\n    OAuth2 / OIDC via login.planet.com\
  \ (Auth0-backed). Authorization Code grant\n    for interactive user sessions (supports MFA and federated login); Client\n    Credentials grant for machine-to-machine (rolling out for api.planet.com,\n    available today for Sentinel Hub services). Access tokens are JWTs presented as\n    `Authorization: Bearer <access_token>`.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.planet.com/authorize\n    tokenUrl: https://login.planet.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.planet.com/oauth/token\n    note: >-\n      Machine-to-machine; for Sentinel Hub services the token endpoint is\n      https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.planet.com/oauth/device/code\n    tokenUrl: https://login.planet.com/oauth/token\n- name: PlanetOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://login.planet.com/.well-known/openid-configuration\n\
  \  description: >-\n    OpenID Connect discovery is published at login.planet.com. Issuer\n    https://login.planet.com/, JWKS at /.well-known/jwks.json.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planet/refs/heads/main/authentication/planet-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Satellite Imagery
- Earth Observation
- Geospatial
- Remote Sensing
- Mapping
- Analytics
- Location
- Data
- GIS
- Company
---
