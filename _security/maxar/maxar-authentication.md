---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maxar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maxar secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Maxar
provider_slug: maxar
scheme_count: 2
schemes:
- description: OAuth2 bearer token obtained from the Authentication Token Service.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/maxar-openapi.yml
  type: http
- description: 'API key for data-related APIs. Cannot be used for Admin or API Key

    management endpoints, which require an OAuth2 bearer token.'
  in: header
  name: apiKeyAuth
  parameter: MAXAR-API-KEY
  sources:
  - openapi/maxar-openapi.yml
  type: apiKey
slug: maxar-authentication
source_filename: maxar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maxar-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer token obtained from the Authentication Token Service.\n  sources:\n  - openapi/maxar-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: MAXAR-API-KEY\n  description: |-\n    API key for data-related APIs. Cannot be used for Admin or API Key\n    management endpoints, which require an OAuth2 bearer token.\n  sources:\n  - openapi/maxar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxar/refs/heads/main/authentication/maxar-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Earth Observation
- Satellite Imagery
- High Resolution
- Geospatial
- 3D
- STAC
- OGC
- WorldView
- Tasking
- Vantor
- Basemaps
- Change Monitoring
---
