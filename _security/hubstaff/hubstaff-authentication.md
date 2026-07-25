---
api_key_in: []
api_specs:
- filename: hubstaff-activities-api-openapi.yml
  format: yaml
  label: Hubstaff Activities API
  slug: hubstaff-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-activities-api-openapi.yml
- filename: hubstaff-app-url-tracking-api-openapi.yml
  format: yaml
  label: Hubstaff App & URL Tracking API
  slug: hubstaff-app-url-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-app-url-tracking-api-openapi.yml
- filename: hubstaff-attendance-api-openapi.yml
  format: yaml
  label: Hubstaff Attendance API
  slug: hubstaff-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-attendance-api-openapi.yml
- filename: hubstaff-client-invoices-api-openapi.yml
  format: yaml
  label: Hubstaff Client Invoices API
  slug: hubstaff-client-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-client-invoices-api-openapi.yml
- filename: hubstaff-clients-api-openapi.yml
  format: yaml
  label: Hubstaff Clients API
  slug: hubstaff-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-clients-api-openapi.yml
- filename: hubstaff-invites-api-openapi.yml
  format: yaml
  label: Hubstaff Invites API
  slug: hubstaff-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-invites-api-openapi.yml
- filename: hubstaff-members-api-openapi.yml
  format: yaml
  label: Hubstaff Members API
  slug: hubstaff-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-members-api-openapi.yml
- filename: hubstaff-organizations-api-openapi.yml
  format: yaml
  label: Hubstaff Organizations API
  slug: hubstaff-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-organizations-api-openapi.yml
- filename: hubstaff-projects-api-openapi.yml
  format: yaml
  label: Hubstaff Projects API
  slug: hubstaff-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-projects-api-openapi.yml
- filename: hubstaff-screenshots-api-openapi.yml
  format: yaml
  label: Hubstaff Screenshots API
  slug: hubstaff-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-screenshots-api-openapi.yml
- filename: hubstaff-tasks-api-openapi.yml
  format: yaml
  label: Hubstaff Tasks API
  slug: hubstaff-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-tasks-api-openapi.yml
- filename: hubstaff-team-payments-api-openapi.yml
  format: yaml
  label: Hubstaff Team Payments API
  slug: hubstaff-team-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-team-payments-api-openapi.yml
- filename: hubstaff-teams-api-openapi.yml
  format: yaml
  label: Hubstaff Teams API
  slug: hubstaff-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-teams-api-openapi.yml
- filename: hubstaff-time-edit-logs-api-openapi.yml
  format: yaml
  label: Hubstaff Time Edit Logs API
  slug: hubstaff-time-edit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-time-edit-logs-api-openapi.yml
- filename: hubstaff-time-entries-api-openapi.yml
  format: yaml
  label: Hubstaff Time Entries API
  slug: hubstaff-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-time-entries-api-openapi.yml
- filename: hubstaff-time-off-api-openapi.yml
  format: yaml
  label: Hubstaff Time Off API
  slug: hubstaff-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-time-off-api-openapi.yml
- filename: hubstaff-timesheets-api-openapi.yml
  format: yaml
  label: Hubstaff Timesheets API
  slug: hubstaff-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-timesheets-api-openapi.yml
- filename: hubstaff-users-api-openapi.yml
  format: yaml
  label: Hubstaff Users API
  slug: hubstaff-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-users-api-openapi.yml
- filename: hubstaff-webhooks-api-openapi.yml
  format: yaml
  label: Hubstaff Webhooks API
  slug: hubstaff-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-webhooks-api-openapi.yml
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
