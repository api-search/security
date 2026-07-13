---
api_key_in:
- header
api_specs:
- filename: flightaware-openapi.yml
  format: yaml
  label: FlightAware AeroAPI
  slug: aeroapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flightaware Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlightAware secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlightAware
provider_slug: flightaware
scheme_count: 1
schemes:
- description: 'Unlike previous versions of AeroAPI, authentication is now controlled by

    an API key that must be set in the header ```x-apikey```. Your

    FlightAware username is not used when authenticating to the API.'
  in: header
  name: ApiKeyAuth
  parameter: x-apikey
  sources:
  - openapi/flightaware-openapi.yml
  type: apiKey
slug: flightaware-authentication
source_filename: flightaware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flightaware-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: |-\n    Unlike previous versions of AeroAPI, authentication is now controlled by\n    an API key that must be set in the header ```x-apikey```. Your\n    FlightAware username is not used when authenticating to the API.\n  sources:\n  - openapi/flightaware-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/authentication/flightaware-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aviation
- Flights
- Flight Tracking
- Mapping
- Radar
- Satellites
- Traffic Control
---
