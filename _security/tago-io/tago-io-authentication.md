---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: TagoIO REST API
  slug: tago-io-rest-api
  spec_type: OpenAPI
  url: https://api.docs.tago.io/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tago Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: TagoIO secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TagoIO
provider_slug: tago-io
scheme_count: 3
schemes:
- description: A Device-Token that is unique to your device. Generate a token by accessing your Device's page.
  in: header
  name: Device-Token
  parameter: Device-Token
  sources:
  - openapi/tago-io-tago-io-rest-api-openapi.yml
  type: apiKey
- description: A Network Token that is unique to your Network. Access Integrations > Network > Tokens to generate a token for your Network.
  in: header
  name: Network-Token
  parameter: Token
  sources:
  - openapi/tago-io-tago-io-rest-api-openapi.yml
  type: apiKey
- description: A Profile token that is unique to your entire profile. Generate in your account settings.
  in: header
  name: Profile-Token
  parameter: Profile-Token
  sources:
  - openapi/tago-io-tago-io-rest-api-openapi.yml
  type: apiKey
slug: tago-io-authentication
source_filename: tago-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tago-io-tago-io-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Device-Token\n  type: apiKey\n  in: header\n  parameter: Device-Token\n  description: A Device-Token that is unique to your device. Generate a token by accessing your\n    Device's page.\n  sources:\n  - openapi/tago-io-tago-io-rest-api-openapi.yml\n- name: Network-Token\n  type: apiKey\n  in: header\n  parameter: Token\n  description: A Network Token that is unique to your Network. Access Integrations > Network\n    > Tokens to generate a token for your Network.\n  sources:\n  - openapi/tago-io-tago-io-rest-api-openapi.yml\n- name: Profile-Token\n  type: apiKey\n  in: header\n  parameter: Profile-Token\n  description: A Profile token that is unique to your entire profile. Generate in your account\n    settings.\n  sources:\n  - openapi/tago-io-tago-io-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tago-io/refs/heads/main/authentication/tago-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- IoT
- Internet of Things
- Devices
- Data Storage
- Dashboards
- Analysis
- Alerts
- MQTT
- Telemetry
---
