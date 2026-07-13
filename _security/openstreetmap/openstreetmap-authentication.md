---
api_key_in: []
api_specs:
- filename: openstreetmap-main-openapi.yml
  format: yaml
  label: OpenStreetMap Main Editing API v0.6
  slug: main-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-main-openapi.yml
- filename: openstreetmap-nominatim-openapi.yml
  format: yaml
  label: OpenStreetMap Nominatim Geocoding API
  slug: nominatim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-nominatim-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Openstreetmap Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OpenStreetMap secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OpenStreetMap
provider_slug: openstreetmap
scheme_count: 1
schemes:
- description: OAuth 2.0 — required for write operations
  flows:
  - authorizationUrl: https://www.openstreetmap.org/oauth2/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://www.openstreetmap.org/oauth2/token
  name: OAuth2
  sources:
  - openapi/openstreetmap-main-openapi.yml
  type: oauth2
slug: openstreetmap-authentication
source_filename: openstreetmap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openstreetmap-main-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.openstreetmap.org/oauth2/authorize\n    tokenUrl: https://www.openstreetmap.org/oauth2/token\n    scopes: 7\n  description: OAuth 2.0 — required for write operations\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/authentication/openstreetmap-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Geospatial
- Mapping
- Open Data
- Geocoding
- Editing
---
