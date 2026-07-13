---
api_key_in:
- header
- query
api_specs:
- filename: fleetmon-openapi.yml
  format: yaml
  label: FleetMon Vessels API (Retired)
  slug: fleetmon-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/openapi/fleetmon-openapi.yml
- filename: fleetmon-openapi.yml
  format: yaml
  label: FleetMon Vessel Positions API (Retired)
  slug: fleetmon-vessel-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/openapi/fleetmon-openapi.yml
- filename: fleetmon-openapi.yml
  format: yaml
  label: FleetMon Port Calls & ETA API (Retired)
  slug: fleetmon-port-calls-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/openapi/fleetmon-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fleetmon Authentication
name_suffix: Authentication
oauth_flows: []
overview: FleetMon secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FleetMon
provider_slug: fleetmon
scheme_count: 3
schemes:
- description: Auth via API-Key Query-Parameter
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/fleetmon-openapi.yml
  type: apiKey
- description: 'Auth via API-Key in ''Authorization'' header field in the form ''Authorization: Token <apikey>'''
  in: header
  name: apikey_authorization_header
  parameter: Authorization
  sources:
  - openapi/fleetmon-openapi.yml
  type: apiKey
- description: Auth via API-Key in 'Api-Key' header field
  in: header
  name: apikey_header
  parameter: Api-Key
  sources:
  - openapi/fleetmon-openapi.yml
  type: apiKey
slug: fleetmon-authentication
source_filename: fleetmon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fleetmon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Auth via API-Key Query-Parameter\n  sources:\n  - openapi/fleetmon-openapi.yml\n- name: apikey_authorization_header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Auth via API-Key in ''Authorization'' header field in the form ''Authorization:\n    Token <apikey>'''\n  sources:\n  - openapi/fleetmon-openapi.yml\n- name: apikey_header\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Auth via API-Key in 'Api-Key' header field\n  sources:\n  - openapi/fleetmon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/authentication/fleetmon-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Vessel Tracking
- Maritime
- AIS
- Ships
- Ports
- Port Calls
- Shipping
- Retired
---
