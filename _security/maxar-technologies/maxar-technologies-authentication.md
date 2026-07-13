---
api_key_in:
- query
api_specs:
- filename: authentication-openapi.yml
  format: yaml
  label: Vantor Hub Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/authentication-openapi.yml
- filename: discovery-openapi.yml
  format: yaml
  label: Vantor Hub Discovery API
  slug: discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/discovery-openapi.yml
- filename: admin-openapi.yml
  format: yaml
  label: Vantor Hub Account Services API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/admin-openapi.yml
- filename: streaming-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Streaming API
  slug: streaming
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/streaming-openapi.yml
- filename: ordering-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Ordering API
  slug: ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/ordering-openapi.yml
- filename: tasking-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Tasking API
  slug: tasking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/tasking-openapi.yml
- filename: monitoring-openapi.yml
  format: yaml
  label: Maxar Geospatial Platform Monitoring API
  slug: monitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/openapi/monitoring-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maxar Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maxar Technologies secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Maxar Technologies
provider_slug: maxar-technologies
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/admin-openapi.yml
  - openapi/authentication-openapi.yml
  - openapi/discovery-openapi.yml
  - openapi/monitoring-openapi.yml
  - openapi/ordering-openapi.yml
  - openapi/streaming-openapi.yml
  - openapi/tasking-openapi.yml
  type: http
- in: query
  name: apiKeyAuth
  parameter: connectid
  sources:
  - openapi/streaming-openapi.yml
  type: apiKey
slug: maxar-technologies-authentication
source_filename: maxar-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/admin-openapi.yml, openapi/authentication-openapi.yml, openapi/discovery-openapi.yml,\n  openapi/monitoring-openapi.yml, openapi/ordering-openapi.yml, openapi/streaming-openapi.yml,\n  openapi/tasking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/admin-openapi.yml\n  - openapi/authentication-openapi.yml\n  - openapi/discovery-openapi.yml\n  - openapi/monitoring-openapi.yml\n  - openapi/ordering-openapi.yml\n  - openapi/streaming-openapi.yml\n  - openapi/tasking-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: connectid\n  sources:\n  - openapi/streaming-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxar-technologies/refs/heads/main/authentication/maxar-technologies-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Satellite Imagery
- Earth Observation
- Geospatial
- Remote Sensing
- Spatial Intelligence
- Defense
- Intelligence
- WorldView
- STAC
- OGC
- WMS
- WMTS
- WFS
- Tasking
- Basemaps
- Vantor
- Lanteris
- Advent International
- Private Equity
---
