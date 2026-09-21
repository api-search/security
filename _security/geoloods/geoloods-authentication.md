---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: geoloods-openapi.json
  format: json
  label: Geoloods API
  slug: geoloods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoloods/refs/heads/main/openapi/geoloods-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Geoloods Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geoloods secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Geoloods
provider_slug: geoloods
scheme_count: 2
schemes:
- description: Live API key header. Preferred form.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/geoloods-openapi.json
  type: apiKey
- description: Live API key query parameter. Alternative to X-API-Key.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/geoloods-openapi.json
  type: apiKey
slug: geoloods-authentication
source_filename: geoloods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: derived\nsource: openapi/geoloods-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Live API key header. Preferred form.\n  sources:\n  - openapi/geoloods-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Live API key query parameter. Alternative to X-API-Key.\n  sources:\n  - openapi/geoloods-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoloods/refs/heads/main/authentication/geoloods-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Geocoding
- Place Search
- Location
- Coordinates
- Mapping
- Geospatial
- Agents
- OpenAPI
- llms-txt
---
