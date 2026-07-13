---
api_key_in:
- header
- query
api_specs:
- filename: doi-usgs-water-openapi.yml
  format: yaml
  label: USGS Water Data APIs
  slug: usgs-water-data-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doi/refs/heads/main/openapi/doi-usgs-water-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Doi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Interior secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Department of Interior
provider_slug: doi
scheme_count: 2
schemes:
- description: Providing your API key gives you higher rate limits when querying our APIs. You can obtain an API key at https://api.waterdata.usgs.gov/signup
  in: header
  name: ApiKeyHeader
  parameter: api_key
  sources:
  - openapi/doi-usgs-water-openapi.yml
  type: apiKey
- description: Providing your API key gives you higher rate limits when querying our APIs. You can obtain an API key at https://api.waterdata.usgs.gov/signup
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/doi-usgs-water-openapi.yml
  type: apiKey
slug: doi-authentication
source_filename: doi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doi-usgs-water-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: Providing your API key gives you higher rate limits when querying our APIs. You\n    can obtain an API key at https://api.waterdata.usgs.gov/signup\n  sources:\n  - openapi/doi-usgs-water-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Providing your API key gives you higher rate limits when querying our APIs. You\n    can obtain an API key at https://api.waterdata.usgs.gov/signup\n  sources:\n  - openapi/doi-usgs-water-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doi/refs/heads/main/authentication/doi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- National Parks
- Federal Lands
- Water Resources
- Wildlife
- Minerals
- Geospatial
- Geology
- Native American Affairs
- Public Lands
---
