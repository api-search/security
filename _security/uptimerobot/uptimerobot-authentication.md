---
anonymous_access: false
api_key_in: []
api_specs:
- filename: uptimerobot-alert-contacts-api-openapi.yml
  format: yaml
  label: UptimeRobot Alert Contacts API
  slug: uptimerobot-alert-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-alert-contacts-api-openapi.yml
- filename: uptimerobot-incidents-api-openapi.yml
  format: yaml
  label: UptimeRobot Incidents API
  slug: uptimerobot-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-incidents-api-openapi.yml
- filename: uptimerobot-integrations-api-openapi.yml
  format: yaml
  label: UptimeRobot Integrations API
  slug: uptimerobot-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-integrations-api-openapi.yml
- filename: uptimerobot-maintenance-windows-api-openapi.yml
  format: yaml
  label: UptimeRobot Maintenance Windows API
  slug: uptimerobot-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-maintenance-windows-api-openapi.yml
- filename: uptimerobot-monitor-groups-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitor Groups API
  slug: uptimerobot-monitor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitor-groups-api-openapi.yml
- filename: uptimerobot-monitors-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitors API
  slug: uptimerobot-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitors-api-openapi.yml
- filename: uptimerobot-monitors-bulk-operations-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitors - Bulk Operations API
  slug: uptimerobot-monitors-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitors-bulk-operations-api-openapi.yml
- filename: uptimerobot-psp-announcements-api-openapi.yml
  format: yaml
  label: UptimeRobot PSP Announcements API
  slug: uptimerobot-psp-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-psp-announcements-api-openapi.yml
- filename: uptimerobot-public-status-pages-api-openapi.yml
  format: yaml
  label: UptimeRobot Public Status Pages API
  slug: uptimerobot-public-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-public-status-pages-api-openapi.yml
- filename: uptimerobot-storm-protection-api-openapi.yml
  format: yaml
  label: UptimeRobot Storm Protection API
  slug: uptimerobot-storm-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-storm-protection-api-openapi.yml
- filename: uptimerobot-tags-api-openapi.yml
  format: yaml
  label: UptimeRobot Tags API
  slug: uptimerobot-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-tags-api-openapi.yml
- filename: uptimerobot-user-api-openapi.yml
  format: yaml
  label: UptimeRobot User API
  slug: uptimerobot-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Uptimerobot Authentication
name_suffix: Authentication
oauth_flows: []
overview: UptimeRobot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UptimeRobot
provider_slug: uptimerobot
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter your API token (without the "Bearer" prefix — it is added automatically).
  name: bearer
  scheme: bearer
  sources:
  - openapi/uptimerobot-openapi.yaml
  type: http
slug: uptimerobot-authentication
source_filename: uptimerobot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/uptimerobot-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter your API token (without the \"Bearer\" prefix — it is added automatically).\n  sources:\n  - openapi/uptimerobot-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/authentication/uptimerobot-authentication.yml
summary_line: http · 1 scheme
tags:
- Uptime Monitoring
- Status Pages
- Incident Management
- API
- DevOps
- Monitoring Integrations
---
