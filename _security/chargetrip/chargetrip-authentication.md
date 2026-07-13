---
api_key_in:
- header
api_specs:
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Route Planning API
  slug: chargetrip-route-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Stations API
  slug: chargetrip-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Car Database API
  slug: chargetrip-car-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Isolines / Reachability API
  slug: chargetrip-isolines-reachability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
- filename: chargetrip-openapi.yml
  format: yaml
  label: Chargetrip Operators API
  slug: chargetrip-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/openapi/chargetrip-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chargetrip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chargetrip secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chargetrip
provider_slug: chargetrip
scheme_count: 2
schemes:
- description: Chargetrip client identifier sent on every request.
  in: header
  name: clientId
  parameter: x-client-id
  sources:
  - openapi/chargetrip-openapi.yml
  type: apiKey
- description: Chargetrip application identifier sent on every request.
  in: header
  name: appId
  parameter: x-app-id
  sources:
  - openapi/chargetrip-openapi.yml
  type: apiKey
slug: chargetrip-authentication
source_filename: chargetrip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chargetrip-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: x-client-id\n  description: Chargetrip client identifier sent on every request.\n  sources:\n  - openapi/chargetrip-openapi.yml\n- name: appId\n  type: apiKey\n  in: header\n  parameter: x-app-id\n  description: Chargetrip application identifier sent on every request.\n  sources:\n  - openapi/chargetrip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargetrip/refs/heads/main/authentication/chargetrip-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- EV
- Routing
- Charging Stations
- GraphQL
- Mobility
---
