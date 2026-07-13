---
api_key_in:
- header
- query
api_specs:
- filename: usgs-earthquake-api-openapi.yaml
  format: yaml
  label: Earthquake Notifications, Feeds, and Web Services
  slug: earthquake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-geological-survey/refs/heads/main/openapi/usgs-earthquake-api-openapi.yaml
- filename: usgs-water-data-api-openapi.yaml
  format: yaml
  label: USGS Water Data APIs
  slug: water-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-geological-survey/refs/heads/main/openapi/usgs-water-data-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: U S Geological Survey Authentication
name_suffix: Authentication
oauth_flows: []
overview: U.S. Geological Survey secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: U.S. Geological Survey
provider_slug: u-s-geological-survey
scheme_count: 2
schemes:
- description: USGS Water Data API key. Obtain at https://api.waterdata.usgs.gov/signup/
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/usgs-water-data-api-openapi.yaml
  type: apiKey
- description: USGS Water Data API key passed as a request header.
  in: header
  name: ApiKeyHeader
  parameter: api_key
  sources:
  - openapi/usgs-water-data-api-openapi.yaml
  type: apiKey
slug: u-s-geological-survey-authentication
source_filename: u-s-geological-survey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usgs-water-data-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: USGS Water Data API key. Obtain at https://api.waterdata.usgs.gov/signup/\n  sources:\n  - openapi/usgs-water-data-api-openapi.yaml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: USGS Water Data API key passed as a request header.\n  sources:\n  - openapi/usgs-water-data-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-geological-survey/refs/heads/main/authentication/u-s-geological-survey-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Geological
- Earth Science
- Natural Resources
- Earthquake
- Water
- Hydrology
---
