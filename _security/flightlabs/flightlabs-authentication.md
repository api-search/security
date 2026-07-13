---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: FlightLabs API
  slug: flightlabs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flightlabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlightLabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlightLabs
provider_slug: flightlabs
scheme_count: 1
schemes:
- description: API key obtained from your FlightLabs dashboard
  in: query
  name: AccessKey
  parameter: access_key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: flightlabs-authentication
source_filename: flightlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: AccessKey\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: API key obtained from your FlightLabs dashboard\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/authentication/flightlabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aviation
- Flights
- Airlines
- Airports
- Flight Tracking
- Travel
- Real-Time Data
---
