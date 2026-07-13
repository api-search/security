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
name: Planet Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Planet Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Planet Labs
provider_slug: planet-labs
scheme_count: 2
schemes:
- description: 'HTTP Basic with the Planet API key as the username and an empty

    password.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/planet-labs-openapi.yml
  type: http
- description: Alternative API key/token header.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/planet-labs-openapi.yml
  type: apiKey
slug: planet-labs-authentication
source_filename: planet-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/planet-labs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic with the Planet API key as the username and an empty\n    password.\n  sources:\n  - openapi/planet-labs-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Alternative API key/token header.\n  sources:\n  - openapi/planet-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planet-labs/refs/heads/main/authentication/planet-labs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Earth Observation
- Satellite Imagery
- Geospatial
- PlanetScope
- SkySat
- Pelican
- Tasking
- Basemaps
- Analytics
- Subscriptions
- STAC
- GIS
---
