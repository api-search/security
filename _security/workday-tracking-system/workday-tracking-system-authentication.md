---
api_key_in: []
api_specs:
- filename: workday-tracking-system-accruals-api-openapi.yml
  format: yaml
  label: Workday Tracking System Accruals API
  slug: workday-tracking-system-accruals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-accruals-api-openapi.yml
- filename: workday-tracking-system-balances-api-openapi.yml
  format: yaml
  label: Workday Tracking System Balances API
  slug: workday-tracking-system-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-balances-api-openapi.yml
- filename: workday-tracking-system-labor-demand-api-openapi.yml
  format: yaml
  label: Workday Tracking System Labor Demand API
  slug: workday-tracking-system-labor-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-labor-demand-api-openapi.yml
- filename: workday-tracking-system-leave-of-absence-api-openapi.yml
  format: yaml
  label: Workday Tracking System Leave of Absence API
  slug: workday-tracking-system-leave-of-absence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-leave-of-absence-api-openapi.yml
- filename: workday-tracking-system-scheduling-organizations-api-openapi.yml
  format: yaml
  label: Workday Tracking System Scheduling Organizations API
  slug: workday-tracking-system-scheduling-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-scheduling-organizations-api-openapi.yml
- filename: workday-tracking-system-shifts-api-openapi.yml
  format: yaml
  label: Workday Tracking System Shifts API
  slug: workday-tracking-system-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-shifts-api-openapi.yml
- filename: workday-tracking-system-time-blocks-api-openapi.yml
  format: yaml
  label: Workday Tracking System Time Blocks API
  slug: workday-tracking-system-time-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-blocks-api-openapi.yml
- filename: workday-tracking-system-time-clock-events-api-openapi.yml
  format: yaml
  label: Workday Tracking System Time Clock Events API
  slug: workday-tracking-system-time-clock-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-clock-events-api-openapi.yml
- filename: workday-tracking-system-time-off-api-openapi.yml
  format: yaml
  label: Workday Tracking System Time Off API
  slug: workday-tracking-system-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-off-api-openapi.yml
- filename: workday-tracking-system-time-requests-api-openapi.yml
  format: yaml
  label: Workday Tracking System Time Requests API
  slug: workday-tracking-system-time-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-requests-api-openapi.yml
- filename: workday-tracking-system-timesheets-api-openapi.yml
  format: yaml
  label: Workday Tracking System Timesheets API
  slug: workday-tracking-system-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-timesheets-api-openapi.yml
- filename: workday-tracking-system-work-schedules-api-openapi.yml
  format: yaml
  label: Workday Tracking System Work Schedules API
  slug: workday-tracking-system-work-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-work-schedules-api-openapi.yml
- filename: workday-tracking-system-worker-preferences-api-openapi.yml
  format: yaml
  label: Workday Tracking System Worker Preferences API
  slug: workday-tracking-system-worker-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-worker-preferences-api-openapi.yml
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
- Payroll
- Scheduling
- Time Tracking
- Timesheets
- Workforce Management
---
