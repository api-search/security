---
api_key_in:
- header
api_specs:
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Timeseries API
  slug: climate-engine-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Zonal Statistics API
  slug: climate-engine-zonal-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Raster API
  slug: climate-engine-raster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Reports API
  slug: climate-engine-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Dataset Catalog API
  slug: climate-engine-dataset-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Account API
  slug: climate-engine-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Climate Engine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Climate Engine secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Climate Engine
provider_slug: climate-engine
scheme_count: 1
schemes:
- description: API key issued by the Climate Engine team, sent in the Authorization header. Request a key from the ClimateEngine.org team.
  in: header
  name: APIKeyHeader
  parameter: Authorization
  sources:
  - openapi/climate-engine-openapi.yml
  type: apiKey
slug: climate-engine-authentication
source_filename: climate-engine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/climate-engine-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key issued by the Climate Engine team, sent in the Authorization header.\n    Request a key from the ClimateEngine.org team.\n  sources:\n  - openapi/climate-engine-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/authentication/climate-engine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Climate
- Geospatial
- Remote Sensing
- Satellite
- Earth Observation
---
