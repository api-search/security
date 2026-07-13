---
api_key_in:
- header
api_specs:
- filename: attom-property-api-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attom-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-property-api-openapi.yml
- filename: attom-area-api-openapi.yml
  format: yaml
  label: ATTOM Area API
  slug: attom-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-area-api-openapi.yml
- filename: attom-poi-api-openapi.yml
  format: yaml
  label: ATTOM POI API
  slug: attom-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-poi-api-openapi.yml
- filename: attom-community-api-openapi.yml
  format: yaml
  label: ATTOM Community API
  slug: attom-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-community-api-openapi.yml
- filename: attom-parcel-tiles-api-openapi.yml
  format: yaml
  label: ATTOM Parcel Tiles API
  slug: attom-parcel-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-parcel-tiles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Attomdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: ATTOM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ATTOM
provider_slug: attomdata
scheme_count: 1
schemes:
- description: ATTOM-issued API key. Pass on every request via the `apikey` header.
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/attom-area-api-openapi.yml
  - openapi/attom-community-api-openapi.yml
  - openapi/attom-parcel-tiles-api-openapi.yml
  - openapi/attom-poi-api-openapi.yml
  - openapi/attom-property-api-openapi.yml
  type: apiKey
slug: attomdata-authentication
source_filename: attomdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/attom-area-api-openapi.yml, openapi/attom-community-api-openapi.yml, openapi/attom-parcel-tiles-api-openapi.yml,\n  openapi/attom-poi-api-openapi.yml, openapi/attom-property-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: ATTOM-issued API key. Pass on every request via the `apikey` header.\n  sources:\n  - openapi/attom-area-api-openapi.yml\n  - openapi/attom-community-api-openapi.yml\n  - openapi/attom-parcel-tiles-api-openapi.yml\n  - openapi/attom-poi-api-openapi.yml\n  - openapi/attom-property-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/authentication/attomdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real Estate
- Property Data
- Property Intelligence
- Mortgage
- Assessment
- AVM
- Foreclosure
- Transactions
- Owner Data
- Building Permits
- Geospatial
- Boundaries
- Demographics
- Neighborhood
- POI
- Insurance
- Mortgage Technology
- PropTech
---
