---
api_key_in:
- query
api_specs:
- filename: esri-arcgis-platform-openapi.yml
  format: yaml
  label: ESRI ArcGIS Platform API
  slug: esri-arcgis-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-platform-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
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
  - openapi/esri-arcgis-platform-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: OAuth2
  sources:
  - openapi/esri-arcgis-platform-openapi.yml
  type: oauth2
slug: esri-arcgis-authentication
source_filename: esri-arcgis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/esri-arcgis-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: ArcGIS API key or token\n  sources:\n  - openapi/esri-arcgis-platform-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/esri-arcgis-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/authentication/esri-arcgis-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- GIS
- Geospatial
- Mapping
- Location
- Spatial Analysis
---
