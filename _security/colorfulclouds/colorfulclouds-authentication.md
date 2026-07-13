---
api_key_in:
- query
api_specs:
- filename: colorfulclouds-caiyun-weather-openapi.yml
  format: yaml
  label: Caiyun Weather API
  slug: caiyun-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colorfulclouds/refs/heads/main/openapi/colorfulclouds-caiyun-weather-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Colorfulclouds Authentication
name_suffix: Authentication
oauth_flows: []
overview: ColorfulClouds secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ColorfulClouds
provider_slug: colorfulclouds
scheme_count: 1
schemes:
- description: Caiyun Weather API token. Note that the token is conventionally embedded in the path between the API version and the lng,lat segment rather than sent as a header or query parameter. This security scheme is recorded for tooling completeness; clients should construct the URL with the token in the path as documented.
  in: query
  name: pathToken
  parameter: token
  sources:
  - openapi/colorfulclouds-caiyun-weather-openapi.yml
  type: apiKey
slug: colorfulclouds-authentication
source_filename: colorfulclouds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/colorfulclouds-caiyun-weather-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: pathToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Caiyun Weather API token. Note that the token is conventionally embedded in the\n    path between the API version and the lng,lat segment rather than sent as a header or query\n    parameter. This security scheme is recorded for tooling completeness; clients should construct\n    the URL with the token in the path as documented.\n  sources:\n  - openapi/colorfulclouds-caiyun-weather-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorfulclouds/refs/heads/main/authentication/colorfulclouds-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Weather
- Forecasting
- Air Quality
- Precipitation
- Hyperlocal
- Geospatial
- China
---
