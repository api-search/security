---
api_key_in: []
api_specs:
- filename: span-rest-api-openapi.json
  format: json
  label: SPAN REST API
  slug: span-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-rest-api-openapi.json
- filename: span-ebus-asyncapi.yml
  format: yaml
  label: SPAN eBus MQTT API
  slug: span-ebus-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/asyncapi/span-ebus-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Span Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: SPAN secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SPAN
provider_slug: span-io
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/span-rest-api-openapi.json
  type: http
slug: span-io-authentication
source_filename: span-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/span-rest-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/span-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/authentication/span-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Home Energy
- Electrification
- Smart Panel
- Electrical Panel
- Home Automation
- Solar
- Energy Storage
- EV Charging
- Grid
- Islanding
- Backup Power
- Demand Response
- IoT
- MQTT
- Homie
- Electrification Bus
- On-Premise
---
