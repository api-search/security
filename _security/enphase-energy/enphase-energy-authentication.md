---
api_key_in:
- header
- query
api_specs:
- filename: enphase-energy-device-level-production-monitoring-api-openapi.yml
  format: yaml
  label: Enphase Energy Device Level Production Monitoring API
  slug: enphase-energy-device-level-production-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-device-level-production-monitoring-api-openapi.yml
- filename: enphase-energy-ev-charger-control-api-openapi.yml
  format: yaml
  label: Enphase Energy EV Charger Control API
  slug: enphase-energy-ev-charger-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-ev-charger-control-api-openapi.yml
- filename: enphase-energy-ev-charger-monitoring-api-openapi.yml
  format: yaml
  label: Enphase Energy EV Charger Monitoring API
  slug: enphase-energy-ev-charger-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-ev-charger-monitoring-api-openapi.yml
- filename: enphase-energy-site-level-consumption-monitoring-api-openapi.yml
  format: yaml
  label: Enphase Energy Site Level Consumption Monitoring API
  slug: enphase-energy-site-level-consumption-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-site-level-consumption-monitoring-api-openapi.yml
- filename: enphase-energy-site-level-production-monitoring-api-openapi.yml
  format: yaml
  label: Enphase Energy Site Level Production Monitoring API
  slug: enphase-energy-site-level-production-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-site-level-production-monitoring-api-openapi.yml
- filename: enphase-energy-streaming-apis-api-openapi.yml
  format: yaml
  label: Enphase Energy Streaming APIs API
  slug: enphase-energy-streaming-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-streaming-apis-api-openapi.yml
- filename: enphase-energy-system-configurations-api-openapi.yml
  format: yaml
  label: Enphase Energy System Configurations API
  slug: enphase-energy-system-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-system-configurations-api-openapi.yml
- filename: enphase-energy-system-details-api-openapi.yml
  format: yaml
  label: Enphase Energy System Details API
  slug: enphase-energy-system-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-system-details-api-openapi.yml
- filename: enphase-energy-systems-api-openapi.yml
  format: yaml
  label: Enphase Energy Systems API
  slug: enphase-energy-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/openapi/enphase-energy-systems-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Enphase Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enphase Energy secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enphase Energy
provider_slug: enphase-energy
scheme_count: 3
schemes:
- in: query
  name: ApiKey
  parameter: key
  sources:
  - openapi/enphase-enlighten-v2-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from Enphase authorization server.
  name: oauth2
  scheme: bearer
  sources:
  - openapi/enphase-enlighten-v4-monitoring-openapi.yml
  type: http
- description: API key associated with your Enphase developer application.
  in: header
  name: apiKey
  parameter: key
  sources:
  - openapi/enphase-enlighten-v4-monitoring-openapi.yml
  type: apiKey
slug: enphase-energy-authentication
source_filename: enphase-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/enphase-enlighten-v2-openapi.yml, openapi/enphase-enlighten-v4-monitoring-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/enphase-enlighten-v2-openapi.yml\n- name: oauth2\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from Enphase authorization server.\n  sources:\n  - openapi/enphase-enlighten-v4-monitoring-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: key\n  description: API key associated with your Enphase developer application.\n  sources:\n  - openapi/enphase-enlighten-v4-monitoring-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enphase-energy/refs/heads/main/authentication/enphase-energy-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Solar
- Energy
- Microinverters
- Battery Storage
- IQ Battery
- IQ Microinverter
- IQ EV Charger
- Enlighten
- Home Energy Management
- Renewable Energy
- Grid Services
- Cleantech
- IoT
- Telemetry
---
