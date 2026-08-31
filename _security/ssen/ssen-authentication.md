---
api_key_in:
- query
api_specs:
- filename: ssen-catalog-api-openapi.yml
  format: yaml
  label: Scottish and Southern Electricity Networks Catalog API
  slug: ssen-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssen/refs/heads/main/openapi/ssen-catalog-api-openapi.yml
- filename: ssen-dataset-api-openapi.yml
  format: yaml
  label: Scottish and Southern Electricity Networks Dataset API
  slug: ssen-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssen/refs/heads/main/openapi/ssen-dataset-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ssen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scottish and Southern Electricity Networks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scottish and Southern Electricity Networks
provider_slug: ssen
scheme_count: 1
schemes:
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/ssen-transmission-opendatasoft-explore-v2.1-openapi.json
  type: apiKey
slug: ssen-authentication
source_filename: ssen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/ssen-transmission-opendatasoft-explore-v2.1-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  sources:\n  - openapi/ssen-transmission-opendatasoft-explore-v2.1-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssen/refs/heads/main/authentication/ssen-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network Operator
- Transmission
- Smart Metering
- Open Data
- Flexibility
- Renewables
- DER
---
