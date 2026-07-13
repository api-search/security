---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: OneBusAway REST API
  slug: onebusaway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/OneBusAway/sdk-config/main/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Onebusaway Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneBusAway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OneBusAway
provider_slug: onebusaway
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: onebusaway-authentication
source_filename: onebusaway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onebusaway/refs/heads/main/authentication/onebusaway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Transit
- Public Transit
- Real-Time
- Arrivals
- Departures
- Bus
- GTFS
- Open Source
- Stop Data
- Trip Planning
- Service Alerts
- Vehicle Positions
- Open Data
---
