---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: esri-arcgis-geocoding-api-openapi.yml
  format: yaml
  label: ESRI ArcGIS Geocoding API
  slug: esri-arcgis-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-geocoding-api-openapi.yml
- filename: esri-arcgis-places-api-openapi.yml
  format: yaml
  label: ESRI ArcGIS Places API
  slug: esri-arcgis-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-places-api-openapi.yml
- filename: esri-arcgis-portal-api-openapi.yml
  format: yaml
  label: ESRI ArcGIS Portal API
  slug: esri-arcgis-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-portal-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Esri Arcgis Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ESRI ArcGIS secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ESRI ArcGIS
provider_slug: esri-arcgis
scheme_count: 2
schemes:
- description: ArcGIS API key or token
  in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/esri-arcgis-geocoding-api-openapi.yml
  - openapi/esri-arcgis-places-api-openapi.yml
  - openapi/esri-arcgis-portal-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: OAuth2
  sources:
  - openapi/esri-arcgis-geocoding-api-openapi.yml
  - openapi/esri-arcgis-places-api-openapi.yml
  - openapi/esri-arcgis-portal-api-openapi.yml
  type: oauth2
slug: esri-arcgis-authentication
source_filename: esri-arcgis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://developers.arcgis.com/documentation/security-and-authentication/, https://www.arcgis.com/.well-known/oauth-authorization-server\n  (HTTP 200), https://location-services-mcp.arcgis.com/.well-known/oauth-protected-resource (HTTP 200); baseline\n  derived from openapi/ securitySchemes\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: ArcGIS API key or token\n  sources:\n  - openapi/esri-arcgis-geocoding-api-openapi.yml\n  - openapi/esri-arcgis-places-api-openapi.yml\n  - openapi/esri-arcgis-portal-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/esri-arcgis-geocoding-api-openapi.yml\n\
  \  - openapi/esri-arcgis-places-api-openapi.yml\n  - openapi/esri-arcgis-portal-api-openapi.yml\ndocs: https://developers.arcgis.com/documentation/security-and-authentication/\nmodels:\n- name: API key authentication\n  type: api-key\n  docs: https://developers.arcgis.com/documentation/security-and-authentication/api-key-authentication/\n  transport:\n  - query parameter token\n  - 'Authorization: Bearer <key>'\n  note: An ArcGIS API key credential is a long-lived access token scoped by PRIVILEGE, chosen when the credential\n    is created. There is no OAuth scope string on this path.\n- name: User authentication (OAuth 2.0)\n  type: oauth2\n  docs: https://developers.arcgis.com/documentation/security-and-authentication/user-authentication/\n  flow: authorizationCode\n  pkce: S256\n  authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n  tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n  note: An app acts on behalf of a signed-in ArcGIS user; the resulting\
  \ token carries that user’s privileges.\n- name: App authentication\n  type: oauth2\n  docs: https://developers.arcgis.com/documentation/security-and-authentication/app-authentication/\n  flow: clientCredentials\n  tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n  note: App-only token for services that do not need a user identity.\ndiscovery:\n  rfc8414:\n    url: https://www.arcgis.com/.well-known/oauth-authorization-server\n    http_status: 200\n    issuer: https://www.arcgis.com\n    grant_types_supported:\n    - authorization_code\n    - implicit\n    response_types_supported:\n    - code\n    - token\n    code_challenge_methods_supported:\n    - S256\n    file: well-known/esri-arcgis-www-arcgis-com-oauth-authorization-server.json\n  rfc9728:\n    url: https://location-services-mcp.arcgis.com/.well-known/oauth-protected-resource\n    http_status: 200\n    resource: https://location-services-mcp.arcgis.com/\n    authorization_servers:\n    - https://arcgis.com/\n    file:\
  \ well-known/esri-arcgis-location-services-mcp-oauth-protected-resource.json\n  openid_configuration:\n    url: https://www.arcgis.com/.well-known/openid-configuration\n    http_status: 404\ntoken_reference: https://developers.arcgis.com/documentation/security-and-authentication/reference/access-tokens/\nprivileges_reference: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/\nnotes:\n- ArcGIS authorizes by PRIVILEGE, not by OAuth scope string. The scope values in the spec (openid, urn:arcgis:scope:root)\n  are coarse; the real permission surface is the privilege list attached to the credential. See scopes/esri-arcgis-scopes.yml.\n- A credential that authenticates but lacks the required privilege returns HTTP 200 with error.code 403 in the body\n  - not a 403 status. See errors/esri-arcgis-problem-types.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/authentication/esri-arcgis-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- GIS
- Geospatial
- Mapping
- Location
- Spatial Analysis
- Geocoding
- Routing
- Places
- OGC
- GraphQL
- MCP
---
