---
api_key_in:
- header
- query
api_specs:
- filename: nagios-xi-openapi.yml
  format: yaml
  label: Nagios XI REST API
  slug: xi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-xi-openapi.yml
- filename: ncpa-openapi.yml
  format: yaml
  label: NCPA (Nagios Cross-Platform Agent) API
  slug: ncpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/ncpa-openapi.yml
- filename: nrdp-openapi.yml
  format: yaml
  label: NRDP (Nagios Remote Data Processor) API
  slug: nrdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nrdp-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nagios Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nagios secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nagios
provider_slug: nagios
scheme_count: 3
schemes:
- in: query
  name: ApiKeyQuery
  parameter: apikey
  sources:
  - openapi/nagios-xi-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/nagios-xi-openapi.yml
  type: apiKey
- in: query
  name: TokenAuth
  parameter: token
  sources:
  - openapi/ncpa-openapi.yml
  - openapi/nrdp-openapi.yml
  type: apiKey
slug: nagios-authentication
source_filename: nagios-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nagios-xi-openapi.yml, openapi/ncpa-openapi.yml, openapi/nrdp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/nagios-xi-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/nagios-xi-openapi.yml\n- name: TokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/ncpa-openapi.yml\n  - openapi/nrdp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/authentication/nagios-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Monitoring
- Infrastructure Monitoring
- Network Monitoring
- Open Source
- IT Operations
- Alerting
- Observability
- Nagios XI
- Nagios Core
- NCPA
- NRPE
- NSCA
- NRDP
---
