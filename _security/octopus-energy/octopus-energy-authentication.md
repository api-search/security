---
api_key_in: []
api_specs:
- filename: octopus-energy-public-api-openapi.yml
  format: yaml
  label: Octopus Energy Public API
  slug: octopus-energy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-energy/refs/heads/main/openapi/octopus-energy-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Octopus Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octopus Energy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Octopus Energy
provider_slug: octopus-energy
scheme_count: 1
schemes:
- description: HTTP Basic authentication with the customer API key as the username and an empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/octopus-energy-public-api-openapi.yml
  type: http
slug: octopus-energy-authentication
source_filename: octopus-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octopus-energy-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with the customer API key as the username and an empty\n    password.\n  sources:\n  - openapi/octopus-energy-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopus-energy/refs/heads/main/authentication/octopus-energy-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Electricity
- Gas
- Renewable Energy
- Smart Meter
- Tariffs
- Kraken
- UK
- DER
- Electric Vehicles
- Heat Pumps
- Solar
- Battery
---
