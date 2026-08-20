---
api_key_in:
- query
api_specs:
- filename: regrid-metadata-api-openapi.yml
  format: yaml
  label: Regrid Metadata API
  slug: regrid-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/openapi/regrid-metadata-api-openapi.yml
- filename: regrid-parcel-query-api-openapi.yml
  format: yaml
  label: Regrid Parcel Query API
  slug: regrid-parcel-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/openapi/regrid-parcel-query-api-openapi.yml
- filename: regrid-parcel-search-api-openapi.yml
  format: yaml
  label: Regrid Parcel Search API
  slug: regrid-parcel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/openapi/regrid-parcel-search-api-openapi.yml
- filename: regrid-schemas-api-openapi.yml
  format: yaml
  label: Regrid Schemas API
  slug: regrid-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/openapi/regrid-schemas-api-openapi.yml
- filename: regrid-typeahead-api-openapi.yml
  format: yaml
  label: Regrid Typeahead API
  slug: regrid-typeahead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/openapi/regrid-typeahead-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Regrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regrid secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Regrid
provider_slug: regrid
scheme_count: 1
schemes:
- description: API token obtained from your Regrid account profile
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/regrid-parcel-openapi.yml
  type: apiKey
slug: regrid-authentication
source_filename: regrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regrid-parcel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token obtained from your Regrid account profile\n  sources:\n  - openapi/regrid-parcel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/authentication/regrid-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Parcels
- Land Data
- Property Data
- GeoJSON
- Real-Estate
- Zoning
- Ownership
- Geospatial
- Mapping
- Tiles
---
