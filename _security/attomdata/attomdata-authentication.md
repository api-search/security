---
api_key_in:
- header
api_specs:
- filename: attomdata-all-events-api-openapi.yml
  format: yaml
  label: ATTOM All Events API
  slug: attomdata-all-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-all-events-api-openapi.yml
- filename: attomdata-assessment-api-openapi.yml
  format: yaml
  label: ATTOM Assessment API
  slug: attomdata-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-assessment-api-openapi.yml
- filename: attomdata-avm-api-openapi.yml
  format: yaml
  label: ATTOM AVM API
  slug: attomdata-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-avm-api-openapi.yml
- filename: attomdata-boundary-api-openapi.yml
  format: yaml
  label: ATTOM Boundary API
  slug: attomdata-boundary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-boundary-api-openapi.yml
- filename: attomdata-building-permits-api-openapi.yml
  format: yaml
  label: ATTOM Building Permits API
  slug: attomdata-building-permits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-building-permits-api-openapi.yml
- filename: attomdata-community-api-openapi.yml
  format: yaml
  label: ATTOM Community API
  slug: attomdata-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-community-api-openapi.yml
- filename: attomdata-hierarchy-api-openapi.yml
  format: yaml
  label: ATTOM Hierarchy API
  slug: attomdata-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-hierarchy-api-openapi.yml
- filename: attomdata-home-equity-api-openapi.yml
  format: yaml
  label: ATTOM Home Equity API
  slug: attomdata-home-equity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-home-equity-api-openapi.yml
- filename: attomdata-location-api-openapi.yml
  format: yaml
  label: ATTOM Location API
  slug: attomdata-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-location-api-openapi.yml
- filename: attomdata-lookup-api-openapi.yml
  format: yaml
  label: ATTOM Lookup API
  slug: attomdata-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-lookup-api-openapi.yml
- filename: attomdata-parcel-tiles-api-openapi.yml
  format: yaml
  label: ATTOM Parcel Tiles API
  slug: attomdata-parcel-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-parcel-tiles-api-openapi.yml
- filename: attomdata-poi-categories-api-openapi.yml
  format: yaml
  label: ATTOM POI Categories API
  slug: attomdata-poi-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-poi-categories-api-openapi.yml
- filename: attomdata-poi-search-api-openapi.yml
  format: yaml
  label: ATTOM POI Search API
  slug: attomdata-poi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-poi-search-api-openapi.yml
- filename: attomdata-pre-foreclosure-api-openapi.yml
  format: yaml
  label: ATTOM Pre-Foreclosure API
  slug: attomdata-pre-foreclosure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-pre-foreclosure-api-openapi.yml
- filename: attomdata-property-api-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attomdata-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-property-api-openapi.yml
- filename: attomdata-sale-api-openapi.yml
  format: yaml
  label: ATTOM Sale API
  slug: attomdata-sale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-sale-api-openapi.yml
- filename: attomdata-sales-trends-api-openapi.yml
  format: yaml
  label: ATTOM Sales Trends API
  slug: attomdata-sales-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-sales-trends-api-openapi.yml
- filename: attomdata-school-api-openapi.yml
  format: yaml
  label: ATTOM School API
  slug: attomdata-school-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attomdata-school-api-openapi.yml
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
- Real-Estate
- Property Data
- Property Intelligence
- Mortgage
- Assessment
- AVM
- Foreclosure
- Transaction
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
