---
api_key_in: []
api_specs:
- filename: site24x7-alarms-api-openapi.yml
  format: yaml
  label: Site24x7 Alarms API
  slug: site24x7-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-alarms-api-openapi.yml
- filename: site24x7-current-status-api-openapi.yml
  format: yaml
  label: Site24x7 Current Status API
  slug: site24x7-current-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-current-status-api-openapi.yml
- filename: site24x7-maintenance-windows-api-openapi.yml
  format: yaml
  label: Site24x7 Maintenance Windows API
  slug: site24x7-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-maintenance-windows-api-openapi.yml
- filename: site24x7-monitor-groups-api-openapi.yml
  format: yaml
  label: Site24x7 Monitor Groups API
  slug: site24x7-monitor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-monitor-groups-api-openapi.yml
- filename: site24x7-monitors-api-openapi.yml
  format: yaml
  label: Site24x7 Monitors API
  slug: site24x7-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-monitors-api-openapi.yml
- filename: site24x7-notification-profiles-api-openapi.yml
  format: yaml
  label: Site24x7 Notification Profiles API
  slug: site24x7-notification-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-notification-profiles-api-openapi.yml
- filename: site24x7-outages-api-openapi.yml
  format: yaml
  label: Site24x7 Outages API
  slug: site24x7-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-outages-api-openapi.yml
- filename: site24x7-reports-api-openapi.yml
  format: yaml
  label: Site24x7 Reports API
  slug: site24x7-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-reports-api-openapi.yml
- filename: site24x7-tags-api-openapi.yml
  format: yaml
  label: Site24x7 Tags API
  slug: site24x7-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-tags-api-openapi.yml
- filename: site24x7-threshold-profiles-api-openapi.yml
  format: yaml
  label: Site24x7 Threshold Profiles API
  slug: site24x7-threshold-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-threshold-profiles-api-openapi.yml
- filename: site24x7-users-api-openapi.yml
  format: yaml
  label: Site24x7 Users API
  slug: site24x7-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/openapi/site24x7-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Site24X7 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Site24x7 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Site24x7
provider_slug: site24x7
scheme_count: 1
schemes:
- bearerFormat: Zoho-oauthtoken
  description: 'OAuth 2.0 token obtained from the Zoho Developer Console. Pass as `Authorization: Zoho-oauthtoken {access_token}`.'
  name: ZohoOAuth
  scheme: bearer
  sources:
  - openapi/site24x7-api-openapi.yml
  type: http
slug: site24x7-authentication
source_filename: site24x7-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/site24x7-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ZohoOAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Zoho-oauthtoken\n  description: 'OAuth 2.0 token obtained from the Zoho Developer Console. Pass as `Authorization:\n    Zoho-oauthtoken {access_token}`.'\n  sources:\n  - openapi/site24x7-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/authentication/site24x7-authentication.yml
summary_line: http · 1 scheme
tags:
- Monitoring
- Observability
- Uptime
- Infrastructure
- Cloud
- APM
- SLA
- Alerts
- Synthetic Monitoring
- Real User Monitoring
- Network Monitoring
- Server Monitoring
- Website Monitoring
- On-Call
- Status Pages
---
