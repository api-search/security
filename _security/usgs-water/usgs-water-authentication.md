---
api_key_in:
- header
- query
api_specs:
- filename: openapi
  format: yaml
  label: USGS OGC Continuous Values API
  slug: ogc-continuous-values
  spec_type: OpenAPI
  url: https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=json
- filename: openapi
  format: yaml
  label: USGS OGC Daily Values API
  slug: ogc-daily-values
  spec_type: OpenAPI
  url: https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=json
- filename: openapi
  format: yaml
  label: USGS OGC Monitoring Locations API
  slug: ogc-monitoring-locations
  spec_type: OpenAPI
  url: https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Usgs Water Authentication
name_suffix: Authentication
oauth_flows: []
overview: USGS Water Services secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: USGS Water Services
provider_slug: usgs-water
scheme_count: 2
schemes:
- description: Providing your API key gives you higher rate limits when querying our APIs. You can obtain an API key at https://api.waterdata.usgs.gov/signup
  in: header
  name: ApiKeyHeader
  parameter: api_key
  sources:
  - openapi/usgs-water-openapi.json
  type: apiKey
- description: Providing your API key gives you higher rate limits when querying our APIs. You can obtain an API key at https://api.waterdata.usgs.gov/signup
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/usgs-water-openapi.json
  type: apiKey
slug: usgs-water-authentication
source_filename: usgs-water-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usgs-water-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: Providing your API key gives you higher rate limits when querying our APIs. You\n    can obtain an API key at https://api.waterdata.usgs.gov/signup\n  sources:\n  - openapi/usgs-water-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Providing your API key gives you higher rate limits when querying our APIs. You\n    can obtain an API key at https://api.waterdata.usgs.gov/signup\n  sources:\n  - openapi/usgs-water-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usgs-water/refs/heads/main/authentication/usgs-water-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Water
- Streamflow
- Groundwater
- Water Quality
- Hydrology
- Environmental
- USGS
- NWIS
- Government
- Open Data
- OGC
---
