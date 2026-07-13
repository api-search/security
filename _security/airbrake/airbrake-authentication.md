---
api_key_in:
- query
api_specs:
- filename: airbrake-openapi.yml
  format: yaml
  label: Airbrake API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/openapi/airbrake-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airbrake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airbrake secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airbrake
provider_slug: airbrake
scheme_count: 1
schemes:
- description: Project key, user key, or user token passed as the `key` query string parameter.
  in: query
  name: ProjectKey
  parameter: key
  sources:
  - openapi/airbrake-openapi.yml
  type: apiKey
slug: airbrake-authentication
source_filename: airbrake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airbrake-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ProjectKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Project key, user key, or user token passed as the `key` query string parameter.\n  sources:\n  - openapi/airbrake-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbrake/refs/heads/main/authentication/airbrake-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Error Monitoring
- Application Performance Monitoring
- Observability
- DevOps
- Logging
- Exception Tracking
---
