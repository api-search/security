---
api_key_in:
- header
api_specs:
- filename: vastdata-vms-openapi.json
  format: json
  label: VAST Management System (VMS) REST API
  slug: vast-management-system-vms-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vastdata/refs/heads/main/openapi/vastdata-vms-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vastdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: VAST Data secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VAST Data
provider_slug: vastdata
scheme_count: 2
schemes:
- description: Send current valid API token in an Authorization header with format Api-Token <token>.
  in: header
  name: ApiToken
  parameter: ApiToken
  sources:
  - openapi/vastdata-vms-openapi.json
  type: apiKey
- description: Basic authentication using VMS user name and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vastdata-vms-openapi.json
  type: http
slug: vastdata-authentication
source_filename: vastdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vastdata-vms-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: ApiToken\n  description: Send current valid API token in an Authorization header with format Api-Token\n    <token>.\n  sources:\n  - openapi/vastdata-vms-openapi.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using VMS user name and password\n  sources:\n  - openapi/vastdata-vms-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vastdata/refs/heads/main/authentication/vastdata-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Infrastructure
- Storage
- Data
- AI
- Database
- Kubernetes
- HPC
---
