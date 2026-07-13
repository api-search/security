---
api_key_in: []
api_specs:
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Thermostat API
  slug: ecobee-thermostat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Thermostat Update and Functions API
  slug: ecobee-thermostat-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Runtime Report API
  slug: ecobee-runtime-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Group API
  slug: ecobee-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Demand Response API
  slug: ecobee-demand-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Hierarchy API
  slug: ecobee-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Meter Report API
  slug: ecobee-meter-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Authorization API
  slug: ecobee-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ecobee Authentication
name_suffix: Authentication
oauth_flows: []
overview: ecobee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ecobee
provider_slug: ecobee
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token passed as `Authorization: Bearer ACCESS_TOKEN` on all data-plane requests to https://api.ecobee.com/1.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ecobee-openapi.yml
  type: http
slug: ecobee-authentication
source_filename: ecobee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ecobee-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 access token passed as `Authorization: Bearer ACCESS_TOKEN` on all\n    data-plane requests to https://api.ecobee.com/1.'\n  sources:\n  - openapi/ecobee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/authentication/ecobee-authentication.yml
summary_line: http · 1 scheme
tags:
- Smart Home
- Thermostat
- IoT
- HVAC
- Energy
- Home Automation
- Demand Response
---
