---
api_key_in: []
api_specs:
- filename: workday-tracking-system-time-tracking-openapi.yml
  format: yaml
  label: Workday Time Tracking API
  slug: workday-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-tracking-openapi.yml
- filename: workday-tracking-system-absence-management-openapi.yml
  format: yaml
  label: Workday Absence Management API
  slug: workday-absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-absence-management-openapi.yml
- filename: workday-tracking-system-scheduling-openapi.yml
  format: yaml
  label: Workday Scheduling API
  slug: workday-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-scheduling-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Workday Tracking System Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workday Tracking System secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workday Tracking System
provider_slug: workday-tracking-system
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/workday-tracking-system-absence-management-openapi.yml
  - openapi/workday-tracking-system-scheduling-openapi.yml
  - openapi/workday-tracking-system-time-tracking-openapi.yml
  type: http
slug: workday-tracking-system-authentication
source_filename: workday-tracking-system-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-tracking-system-absence-management-openapi.yml, openapi/workday-tracking-system-scheduling-openapi.yml,\n  openapi/workday-tracking-system-time-tracking-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token authentication\n  sources:\n  - openapi/workday-tracking-system-absence-management-openapi.yml\n  - openapi/workday-tracking-system-scheduling-openapi.yml\n  - openapi/workday-tracking-system-time-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/authentication/workday-tracking-system-authentication.yml
summary_line: http · 1 scheme
tags:
- Absence Management
- Attendance
- Enterprise
- HCM
- Human Capital Management
- Payroll
- Scheduling
- Time Tracking
- Timesheets
- Workforce Management
---
