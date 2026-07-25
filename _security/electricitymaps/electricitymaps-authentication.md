---
api_key_in:
- header
api_specs:
- filename: electricitymaps-carbon-intensity-api-openapi.yml
  format: yaml
  label: Electricity Maps Carbon Intensity API
  slug: electricitymaps-carbon-intensity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-carbon-intensity-api-openapi.yml
- filename: electricitymaps-forecast-api-openapi.yml
  format: yaml
  label: Electricity Maps Forecast API
  slug: electricitymaps-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-forecast-api-openapi.yml
- filename: electricitymaps-health-api-openapi.yml
  format: yaml
  label: Electricity Maps Health API
  slug: electricitymaps-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-health-api-openapi.yml
- filename: electricitymaps-power-breakdown-api-openapi.yml
  format: yaml
  label: Electricity Maps Power Breakdown API
  slug: electricitymaps-power-breakdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-power-breakdown-api-openapi.yml
- filename: electricitymaps-power-consumption-api-openapi.yml
  format: yaml
  label: Electricity Maps Power Consumption API
  slug: electricitymaps-power-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-power-consumption-api-openapi.yml
- filename: electricitymaps-power-production-api-openapi.yml
  format: yaml
  label: Electricity Maps Power Production API
  slug: electricitymaps-power-production-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-power-production-api-openapi.yml
- filename: electricitymaps-zones-api-openapi.yml
  format: yaml
  label: Electricity Maps Zones API
  slug: electricitymaps-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/openapi/electricitymaps-zones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Electricitymaps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electricity Maps secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Electricity Maps
provider_slug: electricitymaps
scheme_count: 1
schemes:
- description: API key issued from the Electricity Maps portal, sent in the auth-token header.
  in: header
  name: authToken
  parameter: auth-token
  sources:
  - openapi/electricitymaps-openapi.yml
  type: apiKey
slug: electricitymaps-authentication
source_filename: electricitymaps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/electricitymaps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: auth-token\n  description: API key issued from the Electricity Maps portal, sent in the auth-token header.\n  sources:\n  - openapi/electricitymaps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electricitymaps/refs/heads/main/authentication/electricitymaps-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Carbon Intensity
- Electricity
- Grid
- Sustainability
---
