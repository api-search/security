---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flightaware-airports-api-openapi.yml
  format: yaml
  label: FlightAware airports API
  slug: flightaware-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-airports-api-openapi.yml
- filename: flightaware-alerts-api-openapi.yml
  format: yaml
  label: FlightAware alerts API
  slug: flightaware-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-alerts-api-openapi.yml
- filename: flightaware-flights-api-openapi.yml
  format: yaml
  label: FlightAware flights API
  slug: flightaware-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-flights-api-openapi.yml
- filename: flightaware-foresight-api-openapi.yml
  format: yaml
  label: FlightAware foresight API
  slug: flightaware-foresight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-foresight-api-openapi.yml
- filename: flightaware-history-api-openapi.yml
  format: yaml
  label: FlightAware history API
  slug: flightaware-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-history-api-openapi.yml
- filename: flightaware-miscellaneous-api-openapi.yml
  format: yaml
  label: FlightAware miscellaneous API
  slug: flightaware-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-miscellaneous-api-openapi.yml
- filename: flightaware-operators-api-openapi.yml
  format: yaml
  label: FlightAware operators API
  slug: flightaware-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-operators-api-openapi.yml
- filename: flightaware-account-api-openapi.yml
  format: yaml
  label: FlightAware Account API
  slug: flightaware-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-account-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
  - openapi/flightaware-account-api-openapi.yml
  - openapi/flightaware-airports-api-openapi.yml
  - openapi/flightaware-alerts-api-openapi.yml
  - openapi/flightaware-flights-api-openapi.yml
  - openapi/flightaware-foresight-api-openapi.yml
  - openapi/flightaware-history-api-openapi.yml
  - openapi/flightaware-miscellaneous-api-openapi.yml
  - openapi/flightaware-operators-api-openapi.yml
  type: apiKey
slug: flightaware-authentication
source_filename: flightaware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: openapi/flightaware-account-api-openapi.yml, openapi/flightaware-airports-api-openapi.yml,\n  openapi/flightaware-alerts-api-openapi.yml, openapi/flightaware-flights-api-openapi.yml, openapi/flightaware-foresight-api-openapi.yml,\n  openapi/flightaware-history-api-openapi.yml, openapi/flightaware-miscellaneous-api-openapi.yml,\n  openapi/flightaware-operators-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: |-\n    Unlike previous versions of AeroAPI, authentication is now controlled by\n    an API key that must be set in the header ```x-apikey```. Your\n    FlightAware username is not used when authenticating to the API.\n  sources:\n  - openapi/flightaware-account-api-openapi.yml\n  - openapi/flightaware-airports-api-openapi.yml\n  - openapi/flightaware-alerts-api-openapi.yml\n  - openapi/flightaware-flights-api-openapi.yml\n\
  \  - openapi/flightaware-foresight-api-openapi.yml\n  - openapi/flightaware-history-api-openapi.yml\n  - openapi/flightaware-miscellaneous-api-openapi.yml\n  - openapi/flightaware-operators-api-openapi.yml\n"
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
