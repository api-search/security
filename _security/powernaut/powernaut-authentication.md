---
api_key_in: []
api_specs:
- filename: powernaut-authentication-api-openapi.yml
  format: yaml
  label: Powernaut authentication API
  slug: powernaut-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-authentication-api-openapi.yml
- filename: powernaut-baselining-api-openapi.yml
  format: yaml
  label: Powernaut baselining API
  slug: powernaut-baselining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-baselining-api-openapi.yml
- filename: powernaut-creating-bids-api-openapi.yml
  format: yaml
  label: Powernaut creating_bids API
  slug: powernaut-creating-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-creating-bids-api-openapi.yml
- filename: powernaut-events-api-openapi.yml
  format: yaml
  label: Powernaut events API
  slug: powernaut-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-events-api-openapi.yml
- filename: powernaut-getting-forecasts-api-openapi.yml
  format: yaml
  label: Powernaut getting_forecasts API
  slug: powernaut-getting-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-getting-forecasts-api-openapi.yml
- filename: powernaut-historical-data-api-openapi.yml
  format: yaml
  label: Powernaut historical_data API
  slug: powernaut-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-historical-data-api-openapi.yml
- filename: powernaut-managing-bids-api-openapi.yml
  format: yaml
  label: Powernaut managing_bids API
  slug: powernaut-managing-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-managing-bids-api-openapi.yml
- filename: powernaut-markets-api-openapi.yml
  format: yaml
  label: Powernaut markets API
  slug: powernaut-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-markets-api-openapi.yml
- filename: powernaut-metrics-api-openapi.yml
  format: yaml
  label: Powernaut metrics API
  slug: powernaut-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-metrics-api-openapi.yml
- filename: powernaut-resources-api-openapi.yml
  format: yaml
  label: Powernaut resources API
  slug: powernaut-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-resources-api-openapi.yml
- filename: powernaut-sensor-data-api-openapi.yml
  format: yaml
  label: Powernaut sensor_data API
  slug: powernaut-sensor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-sensor-data-api-openapi.yml
- filename: powernaut-sites-api-openapi.yml
  format: yaml
  label: Powernaut sites API
  slug: powernaut-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-sites-api-openapi.yml
- filename: powernaut-uploading-forecasts-api-openapi.yml
  format: yaml
  label: Powernaut uploading_forecasts API
  slug: powernaut-uploading-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-uploading-forecasts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Powernaut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Powernaut secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Powernaut
provider_slug: powernaut
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: A bearer token obtained from the token endpoint.
  name: cloud-cloud
  scheme: bearer
  sources:
  - openapi/powernaut-partner-api-openapi-original.yml
  type: http
- description: Your client id and secret to obtain a bearer token for cloud-cloud authentication.
  name: token
  scheme: basic
  sources:
  - openapi/powernaut-partner-api-openapi-original.yml
  type: http
slug: powernaut-authentication
source_filename: powernaut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/powernaut-partner-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: cloud-cloud\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A bearer token obtained from the token endpoint.\n  sources:\n  - openapi/powernaut-partner-api-openapi-original.yml\n- name: token\n  type: http\n  scheme: basic\n  description: Your client id and secret to obtain a bearer token for cloud-cloud authentication.\n  sources:\n  - openapi/powernaut-partner-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/authentication/powernaut-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Energy
- Virtual Power Plant
- Distributed Energy Resources
- Energy Trading
- Flexibility
- Forecasting
- Grid
---
