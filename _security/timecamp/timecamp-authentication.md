---
api_key_in: []
api_specs:
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Time Entries API
  slug: timecamp-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Timer API
  slug: timecamp-timer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Tasks and Projects API
  slug: timecamp-tasks-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Users and Groups API
  slug: timecamp-users-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Attendance API
  slug: timecamp-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Timesheet Approvals API
  slug: timecamp-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Computer Activities API
  slug: timecamp-computer-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Tags API
  slug: timecamp-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Billing Rates and Expenses API
  slug: timecamp-billing-rates-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Data Export API
  slug: timecamp-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Timecamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: TimeCamp secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TimeCamp
provider_slug: timecamp
scheme_count: 2
schemes:
- name: api_key_in_header
  scheme: bearer
  sources:
  - openapi/timecamp-openapi.yml
  type: http
- name: OIDC
  openIdConnectUrl: authenticate/oidc
  sources:
  - openapi/timecamp-openapi.yml
  type: openIdConnect
slug: timecamp-authentication
source_filename: timecamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/timecamp-openapi.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: api_key_in_header\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/timecamp-openapi.yml\n- name: OIDC\n  type: openIdConnect\n  openIdConnectUrl: authenticate/oidc\n  sources:\n  - openapi/timecamp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/authentication/timecamp-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Time Tracking
- Timesheets
- Productivity
- Attendance
- Project Management
- Billing
---
