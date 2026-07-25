---
api_key_in: []
api_specs:
- filename: span-ebus-asyncapi.yml
  format: yaml
  label: SPAN eBus MQTT API
  slug: span-ebus-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/asyncapi/span-ebus-asyncapi.yml
- filename: span-io-auth-api-openapi.yml
  format: yaml
  label: SPAN Auth API
  slug: span-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-auth-api-openapi.yml
- filename: span-io-circuits-api-openapi.yml
  format: yaml
  label: SPAN Circuits API
  slug: span-io-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-circuits-api-openapi.yml
- filename: span-io-islanding-state-api-openapi.yml
  format: yaml
  label: SPAN Islanding State API
  slug: span-io-islanding-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-islanding-state-api-openapi.yml
- filename: span-io-panel-api-openapi.yml
  format: yaml
  label: SPAN Panel API
  slug: span-io-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-panel-api-openapi.yml
- filename: span-io-spaces-api-openapi.yml
  format: yaml
  label: SPAN Spaces API
  slug: span-io-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-spaces-api-openapi.yml
- filename: span-io-status-api-openapi.yml
  format: yaml
  label: SPAN Status API
  slug: span-io-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-status-api-openapi.yml
- filename: span-io-storage-api-openapi.yml
  format: yaml
  label: SPAN Storage API
  slug: span-io-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-storage-api-openapi.yml
- filename: span-io-wifi-api-openapi.yml
  format: yaml
  label: SPAN Wifi API
  slug: span-io-wifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-io-wifi-api-openapi.yml
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
