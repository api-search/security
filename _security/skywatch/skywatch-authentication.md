---
api_key_in:
- header
api_specs:
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Archive Search API
  slug: skywatch-archive-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Pipelines API
  slug: skywatch-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Interval Results & Delivery API
  slug: skywatch-interval-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Cost Estimation API
  slug: skywatch-cost-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Outputs & Bands API
  slug: skywatch-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Locations API
  slug: skywatch-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
- filename: skywatch-openapi.yml
  format: yaml
  label: SkyWatch EarthCache Subscriptions & Callbacks API
  slug: skywatch-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/openapi/skywatch-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Skywatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkyWatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SkyWatch
provider_slug: skywatch
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/skywatch-openapi.yml
  type: apiKey
slug: skywatch-authentication
source_filename: skywatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/skywatch-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/skywatch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skywatch/refs/heads/main/authentication/skywatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Satellite Imagery
- Earth Observation
- Geospatial
- Remote Sensing
- EarthCache
- Imagery
---
