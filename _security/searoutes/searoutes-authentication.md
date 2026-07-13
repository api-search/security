---
api_key_in:
- header
api_specs:
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Ocean Routing API
  slug: searoutes-ocean-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Geocoding API
  slug: searoutes-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes CO2 Emissions API
  slug: searoutes-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Vessel Tracking API
  slug: searoutes-vessel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Search & Carriers API
  slug: searoutes-search-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Weather API
  slug: searoutes-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Searoutes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Searoutes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Searoutes
provider_slug: searoutes
scheme_count: 1
schemes:
- description: API key issued on signup and shown on the developer documentation authentication page. Pass it in the x-api-key request header.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/searoutes-openapi.yml
  type: apiKey
slug: searoutes-authentication
source_filename: searoutes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/searoutes-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued on signup and shown on the developer documentation authentication\n    page. Pass it in the x-api-key request header.\n  sources:\n  - openapi/searoutes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/authentication/searoutes-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Maritime
- Sea Routing
- Ocean Freight
- CO2 Emissions
- Carbon Accounting
- Vessel Tracking
- AIS
- Geocoding
- Logistics
- Supply Chain
---
