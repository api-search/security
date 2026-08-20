---
api_key_in:
- header
- query
api_specs:
- filename: nagios-config-api-openapi.yml
  format: yaml
  label: Nagios Config API
  slug: nagios-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-config-api-openapi.yml
- filename: nagios-cpu-api-openapi.yml
  format: yaml
  label: Nagios CPU API
  slug: nagios-cpu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-cpu-api-openapi.yml
- filename: nagios-disk-api-openapi.yml
  format: yaml
  label: Nagios Disk API
  slug: nagios-disk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-disk-api-openapi.yml
- filename: nagios-interface-api-openapi.yml
  format: yaml
  label: Nagios Interface API
  slug: nagios-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-interface-api-openapi.yml
- filename: nagios-memory-api-openapi.yml
  format: yaml
  label: Nagios Memory API
  slug: nagios-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-memory-api-openapi.yml
- filename: nagios-objects-api-openapi.yml
  format: yaml
  label: Nagios Objects API
  slug: nagios-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-objects-api-openapi.yml
- filename: nagios-plugins-api-openapi.yml
  format: yaml
  label: Nagios Plugins API
  slug: nagios-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-plugins-api-openapi.yml
- filename: nagios-processes-api-openapi.yml
  format: yaml
  label: Nagios Processes API
  slug: nagios-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-processes-api-openapi.yml
- filename: nagios-services-api-openapi.yml
  format: yaml
  label: Nagios Services API
  slug: nagios-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-services-api-openapi.yml
- filename: nagios-submission-api-openapi.yml
  format: yaml
  label: Nagios Submission API
  slug: nagios-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-submission-api-openapi.yml
- filename: nagios-system-api-openapi.yml
  format: yaml
  label: Nagios System API
  slug: nagios-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/openapi/nagios-system-api-openapi.yml
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
- Open-Source
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
