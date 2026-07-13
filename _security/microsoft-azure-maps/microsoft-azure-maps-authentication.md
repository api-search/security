---
api_key_in:
- query
api_specs:
- filename: microsoft-azure-maps-openapi.yml
  format: yaml
  label: Azure Maps Search API
  slug: azure-maps-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-maps/refs/heads/main/openapi/microsoft-azure-maps-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Maps Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Maps secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Maps
provider_slug: microsoft-azure-maps
scheme_count: 2
schemes:
- in: query
  name: subscriptionKey
  parameter: subscription-key
  sources:
  - openapi/microsoft-azure-maps-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-maps-openapi.yml
  type: oauth2
slug: microsoft-azure-maps-authentication
source_filename: microsoft-azure-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-maps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - implicit\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/microsoft-azure-maps-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/microsoft-azure-maps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-maps/refs/heads/main/authentication/microsoft-azure-maps-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Geocoding
- Geospatial
- Location
- Maps
- Mobility
- Routing
- Traffic
- Weather
---
