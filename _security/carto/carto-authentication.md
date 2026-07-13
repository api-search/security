---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Carto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Carto
provider_slug: carto
scheme_count: 1
schemes:
- description: CARTO API Access Token (or OAuth M2M token)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/carto-openapi.yml
  type: http
slug: carto-authentication
source_filename: carto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/carto-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: CARTO API Access Token (or OAuth M2M token)\n  sources:\n  - openapi/carto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carto/refs/heads/main/authentication/carto-authentication.yml
summary_line: http · 1 scheme
tags:
- Location Intelligence
- Geospatial
- Mapping
- GIS
- SQL
- BigQuery
- Snowflake
- Data Warehouse
---
