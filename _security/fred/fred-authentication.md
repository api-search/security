---
api_key_in:
- query
api_specs:
- filename: fred-openapi.yml
  format: yaml
  label: FRED API
  slug: fred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-openapi.yml
- filename: fred-geofred-openapi.yml
  format: yaml
  label: FRED Maps API (GeoFRED)
  slug: fred-maps-api-geofred
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-geofred-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fred Authentication
name_suffix: Authentication
oauth_flows: []
overview: FRED secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FRED
provider_slug: fred
scheme_count: 1
schemes:
- description: 32-character lower-case alphanumeric FRED API key (same key used for the FRED API).
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/fred-geofred-openapi.yml
  - openapi/fred-openapi.yml
  type: apiKey
slug: fred-authentication
source_filename: fred-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fred-geofred-openapi.yml, openapi/fred-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 32-character lower-case alphanumeric FRED API key (same key used for the FRED\n    API).\n  sources:\n  - openapi/fred-geofred-openapi.yml\n  - openapi/fred-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/authentication/fred-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Government
- Economic Data
- Federal Reserve
- Time Series
- Open Data
- Public APIs
---
