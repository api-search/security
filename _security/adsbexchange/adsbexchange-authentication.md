---
api_key_in:
- header
api_specs:
- filename: adsbexchange-geopolitical-filtering-api-openapi.yml
  format: yaml
  label: ADS-B Exchange Geopolitical Filtering API
  slug: adsbexchange-geopolitical-filtering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/adsbexchange-geopolitical-filtering-api-openapi.yml
- filename: adsbexchange-geospatial-filtering-api-openapi.yml
  format: yaml
  label: ADS-B Exchange Geospatial Filtering API
  slug: adsbexchange-geospatial-filtering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/adsbexchange-geospatial-filtering-api-openapi.yml
- filename: adsbexchange-live-positional-data-api-openapi.yml
  format: yaml
  label: ADS-B Exchange Live Positional Data API
  slug: adsbexchange-live-positional-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/adsbexchange-live-positional-data-api-openapi.yml
- filename: adsbexchange-operations-api-openapi.yml
  format: yaml
  label: ADS-B Exchange Operations API
  slug: adsbexchange-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/adsbexchange-operations-api-openapi.yml
- filename: adsbexchange-traces-api-openapi.yml
  format: yaml
  label: ADS-B Exchange Traces API
  slug: adsbexchange-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/adsbexchange-traces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Adsbexchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADS-B Exchange secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ADS-B Exchange
provider_slug: adsbexchange
scheme_count: 1
schemes:
- description: Provide your API key via x-api-key header to access the API.
  in: header
  name: X-Api-Key
  parameter: x-api-key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: adsbexchange-authentication
source_filename: adsbexchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Provide your API key via x-api-key header to access the API.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/authentication/adsbexchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aviation
- Flight Tracking
- ADS-B
- Aircraft
- Real-Time
- Military
- MLAT
---
