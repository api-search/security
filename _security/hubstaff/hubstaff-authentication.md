---
api_key_in: []
api_specs:
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Activities and Time Tracking API
  slug: hubstaff-activities-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Timesheets and Time Entries API
  slug: hubstaff-timesheets-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Organizations and Teams API
  slug: hubstaff-organizations-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Projects and Tasks API
  slug: hubstaff-projects-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Users API
  slug: hubstaff-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Time Off and Attendance API
  slug: hubstaff-time-off-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Clients, Invoices, and Payments API
  slug: hubstaff-clients-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Screenshots and App Tracking API
  slug: hubstaff-screenshots-app-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Webhooks API
  slug: hubstaff-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hubstaff Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hubstaff secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hubstaff
provider_slug: hubstaff
scheme_count: 2
schemes:
- description: Hubstaff Account OpenID Connect / OAuth 2.0 authentication. Scopes are hubstaff:read and hubstaff:write.
  flows:
  - authorizationUrl: https://account.hubstaff.com/authorizations/new
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://account.hubstaff.com/access_tokens
  name: oauth2
  sources:
  - openapi/hubstaff-openapi.yml
  type: oauth2
- description: Access token obtained by exchanging a personal access token (created at https://developer.hubstaff.com/personal_access_tokens) via the OAuth 2.0 refresh token grant at https://account.hubstaff.com/access_tokens. PATs expire after 90 days.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/hubstaff-openapi.yml
  type: http
slug: hubstaff-authentication
source_filename: hubstaff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hubstaff-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.hubstaff.com/authorizations/new\n    tokenUrl: https://account.hubstaff.com/access_tokens\n    scopes: 2\n  description: Hubstaff Account OpenID Connect / OAuth 2.0 authentication. Scopes are hubstaff:read\n    and hubstaff:write.\n  sources:\n  - openapi/hubstaff-openapi.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: Access token obtained by exchanging a personal access token (created at https://developer.hubstaff.com/personal_access_tokens)\n    via the OAuth 2.0 refresh token grant at https://account.hubstaff.com/access_tokens. PATs\n    expire after 90 days.\n  sources:\n  - openapi/hubstaff-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/authentication/hubstaff-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Time Tracking
- Timesheets
- Workforce Management
- Productivity
- Employee Monitoring
- Project Management
- Payroll
---
