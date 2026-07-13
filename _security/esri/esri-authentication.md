---
api_key_in:
- query
api_specs:
- filename: esri-openapi.yml
  format: yaml
  label: Esri ArcGIS Platform API
  slug: esri-arcgis-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Esri Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Esri secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Esri
provider_slug: esri
scheme_count: 2
schemes:
- description: 'ArcGIS Platform API key or access token passed as the `token` query parameter (or `Authorization: Bearer <token>` header on REST services).'
  in: query
  name: apiKeyAuth
  parameter: token
  sources:
  - openapi/esri-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: oauth2
  sources:
  - openapi/esri-openapi.yml
  type: oauth2
slug: esri-authentication
source_filename: esri-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/esri-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: 'ArcGIS Platform API key or access token passed as the `token` query parameter\n    (or `Authorization: Bearer <token>` header on REST services).'\n  sources:\n  - openapi/esri-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/esri-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/authentication/esri-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Geographic
- Geospatial
- GIS
- Location
- Mapping
- Maps
- Spatial Analysis
---
