---
api_key_in:
- header
- path
api_specs:
- filename: solarwinds-orion-openapi.yml
  format: yaml
  label: SolarWinds Orion API
  slug: solarwinds-orion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-orion-openapi.yml
- filename: solarwinds-service-desk-openapi.yml
  format: yaml
  label: SolarWinds Service Desk API
  slug: solarwinds-service-desk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-service-desk-openapi.yml
- filename: openapi.json
  format: json
  label: SolarWinds Observability API
  slug: solarwinds-observability-api
  spec_type: OpenAPI
  url: https://api.na-01.cloud.solarwinds.com/v1/openapi.json
- filename: solarwinds-pingdom-openapi.yml
  format: yaml
  label: SolarWinds Pingdom API
  slug: solarwinds-pingdom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-pingdom-openapi.yml
- filename: solarwinds-loggly-openapi.yml
  format: yaml
  label: SolarWinds Loggly API
  slug: solarwinds-loggly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-loggly-openapi.yml
- filename: solarwinds-papertrail-openapi.yml
  format: yaml
  label: SolarWinds Papertrail API
  slug: solarwinds-papertrail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-papertrail-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Solarwinds Authentication
name_suffix: Authentication
oauth_flows: []
overview: SolarWinds secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SolarWinds
provider_slug: solarwinds
scheme_count: 4
schemes:
- description: API token for authentication via Authorization Bearer header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/solarwinds-loggly-openapi.yml
  - openapi/solarwinds-pingdom-openapi.yml
  - openapi/solarwinds-service-desk-openapi.yml
  type: http
- description: Customer token for event submission endpoints
  in: path
  name: customerToken
  parameter: token
  sources:
  - openapi/solarwinds-loggly-openapi.yml
  type: apiKey
- description: HTTP Basic authentication using Orion Platform credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/solarwinds-orion-openapi.yml
  type: http
- description: Papertrail API token
  in: header
  name: apiToken
  parameter: X-Papertrail-Token
  sources:
  - openapi/solarwinds-papertrail-openapi.yml
  type: apiKey
slug: solarwinds-authentication
source_filename: solarwinds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/solarwinds-loggly-openapi.yml, openapi/solarwinds-orion-openapi.yml, openapi/solarwinds-papertrail-openapi.yml,\n  openapi/solarwinds-pingdom-openapi.yml, openapi/solarwinds-service-desk-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - path\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token for authentication via Authorization Bearer header\n  sources:\n  - openapi/solarwinds-loggly-openapi.yml\n  - openapi/solarwinds-pingdom-openapi.yml\n  - openapi/solarwinds-service-desk-openapi.yml\n- name: customerToken\n  type: apiKey\n  in: path\n  parameter: token\n  description: Customer token for event submission endpoints\n  sources:\n  - openapi/solarwinds-loggly-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using Orion Platform credentials\n  sources:\n  - openapi/solarwinds-orion-openapi.yml\n\
  - name: apiToken\n  type: apiKey\n  in: header\n  parameter: X-Papertrail-Token\n  description: Papertrail API token\n  sources:\n  - openapi/solarwinds-papertrail-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/authentication/solarwinds-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
---
