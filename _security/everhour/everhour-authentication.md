---
api_key_in:
- header
api_specs:
- filename: everhour-clients-api-openapi.yml
  format: yaml
  label: Everhour Clients API
  slug: everhour-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-clients-api-openapi.yml
- filename: everhour-expenses-api-openapi.yml
  format: yaml
  label: Everhour Expenses API
  slug: everhour-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-expenses-api-openapi.yml
- filename: everhour-invoices-api-openapi.yml
  format: yaml
  label: Everhour Invoices API
  slug: everhour-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-invoices-api-openapi.yml
- filename: everhour-projects-api-openapi.yml
  format: yaml
  label: Everhour Projects API
  slug: everhour-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-projects-api-openapi.yml
- filename: everhour-reports-api-openapi.yml
  format: yaml
  label: Everhour Reports API
  slug: everhour-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-reports-api-openapi.yml
- filename: everhour-schedule-api-openapi.yml
  format: yaml
  label: Everhour Schedule API
  slug: everhour-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-schedule-api-openapi.yml
- filename: everhour-tasks-api-openapi.yml
  format: yaml
  label: Everhour Tasks API
  slug: everhour-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-tasks-api-openapi.yml
- filename: everhour-time-off-api-openapi.yml
  format: yaml
  label: Everhour Time Off API
  slug: everhour-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-time-off-api-openapi.yml
- filename: everhour-time-records-api-openapi.yml
  format: yaml
  label: Everhour Time Records API
  slug: everhour-time-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-time-records-api-openapi.yml
- filename: everhour-timecards-api-openapi.yml
  format: yaml
  label: Everhour Timecards API
  slug: everhour-timecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-timecards-api-openapi.yml
- filename: everhour-timers-api-openapi.yml
  format: yaml
  label: Everhour Timers API
  slug: everhour-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-timers-api-openapi.yml
- filename: everhour-timesheets-api-openapi.yml
  format: yaml
  label: Everhour Timesheets API
  slug: everhour-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-timesheets-api-openapi.yml
- filename: everhour-users-api-openapi.yml
  format: yaml
  label: Everhour Users API
  slug: everhour-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-users-api-openapi.yml
- filename: everhour-webhooks-api-openapi.yml
  format: yaml
  label: Everhour Webhooks API
  slug: everhour-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Everhour Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everhour secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Everhour
provider_slug: everhour
scheme_count: 1
schemes:
- description: API key from the bottom of your Everhour profile page.
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/everhour-openapi.yml
  type: apiKey
slug: everhour-authentication
source_filename: everhour-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/everhour-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key from the bottom of your Everhour profile page.\n  sources:\n  - openapi/everhour-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/authentication/everhour-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Time Tracking
- Timesheets
- Productivity
- Project Management
- Budgeting
- Invoicing
---
