---
api_key_in:
- header
api_specs:
- filename: flightaware-aeroapi-openapi.yml
  format: yaml
  label: FlightAware AeroAPI
  slug: flightaware-aeroapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockwell-collins/refs/heads/main/openapi/flightaware-aeroapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rockwell Collins Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rockwell Collins secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rockwell Collins
provider_slug: rockwell-collins
scheme_count: 1
schemes:
- description: 'Unlike previous versions of AeroAPI, authentication is now controlled by

    an API key that must be set in the header ```x-apikey```. Your

    FlightAware username is not used when authenticating to the API.'
  in: header
  name: ApiKeyAuth
  parameter: x-apikey
  sources:
  - openapi/flightaware-aeroapi-openapi.yml
  type: apiKey
slug: rockwell-collins-authentication
source_filename: rockwell-collins-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flightaware-aeroapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: |-\n    Unlike previous versions of AeroAPI, authentication is now controlled by\n    an API key that must be set in the header ```x-apikey```. Your\n    FlightAware username is not used when authenticating to the API.\n  sources:\n  - openapi/flightaware-aeroapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockwell-collins/refs/heads/main/authentication/rockwell-collins-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Avionics
- Aerospace
- Defense
- Aviation
- Flight Deck
- Fortune 500
---
