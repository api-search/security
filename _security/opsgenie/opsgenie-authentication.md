---
api_key_in:
- header
api_specs:
- filename: opsgenie-account-api-openapi.yml
  format: yaml
  label: OpsGenie Account API
  slug: opsgenie-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-account-api-openapi.yml
- filename: opsgenie-alerts-api-openapi.yml
  format: yaml
  label: OpsGenie Alerts API
  slug: opsgenie-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-alerts-api-openapi.yml
- filename: opsgenie-escalations-api-openapi.yml
  format: yaml
  label: OpsGenie Escalations API
  slug: opsgenie-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-escalations-api-openapi.yml
- filename: opsgenie-heartbeats-api-openapi.yml
  format: yaml
  label: OpsGenie Heartbeats API
  slug: opsgenie-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-heartbeats-api-openapi.yml
- filename: opsgenie-incidents-api-openapi.yml
  format: yaml
  label: OpsGenie Incidents API
  slug: opsgenie-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-incidents-api-openapi.yml
- filename: opsgenie-integrations-api-openapi.yml
  format: yaml
  label: OpsGenie Integrations API
  slug: opsgenie-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-integrations-api-openapi.yml
- filename: opsgenie-maintenance-api-openapi.yml
  format: yaml
  label: OpsGenie Maintenance API
  slug: opsgenie-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-maintenance-api-openapi.yml
- filename: opsgenie-notification-rules-api-openapi.yml
  format: yaml
  label: OpsGenie Notification Rules API
  slug: opsgenie-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-notification-rules-api-openapi.yml
- filename: opsgenie-on-call-api-openapi.yml
  format: yaml
  label: OpsGenie On-Call API
  slug: opsgenie-on-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-on-call-api-openapi.yml
- filename: opsgenie-overrides-api-openapi.yml
  format: yaml
  label: OpsGenie Overrides API
  slug: opsgenie-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-overrides-api-openapi.yml
- filename: opsgenie-rotations-api-openapi.yml
  format: yaml
  label: OpsGenie Rotations API
  slug: opsgenie-rotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-rotations-api-openapi.yml
- filename: opsgenie-schedules-api-openapi.yml
  format: yaml
  label: OpsGenie Schedules API
  slug: opsgenie-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-schedules-api-openapi.yml
- filename: opsgenie-services-api-openapi.yml
  format: yaml
  label: OpsGenie Services API
  slug: opsgenie-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-services-api-openapi.yml
- filename: opsgenie-teams-api-openapi.yml
  format: yaml
  label: OpsGenie Teams API
  slug: opsgenie-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-teams-api-openapi.yml
- filename: opsgenie-users-api-openapi.yml
  format: yaml
  label: OpsGenie Users API
  slug: opsgenie-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opsgenie Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpsGenie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpsGenie
provider_slug: opsgenie
scheme_count: 1
schemes:
- description: API key authentication using the GenieKey scheme.
  in: header
  name: genieKey
  parameter: Authorization
  sources:
  - openapi/opsgenie-account-openapi.yml
  - openapi/opsgenie-alert-openapi.yml
  - openapi/opsgenie-escalation-openapi.yml
  - openapi/opsgenie-heartbeat-openapi.yml
  - openapi/opsgenie-incident-openapi.yml
  - openapi/opsgenie-integration-openapi.yml
  - openapi/opsgenie-maintenance-openapi.yml
  - openapi/opsgenie-notification-rule-openapi.yml
  - openapi/opsgenie-schedule-openapi.yml
  - openapi/opsgenie-service-openapi.yml
  - openapi/opsgenie-team-openapi.yml
  - openapi/opsgenie-user-openapi.yml
  type: apiKey
slug: opsgenie-authentication
source_filename: opsgenie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opsgenie-account-openapi.yml, openapi/opsgenie-alert-openapi.yml, openapi/opsgenie-escalation-openapi.yml,\n  openapi/opsgenie-heartbeat-openapi.yml, openapi/opsgenie-incident-openapi.yml, openapi/opsgenie-integration-openapi.yml,\n  openapi/opsgenie-maintenance-openapi.yml, openapi/opsgenie-notification-rule-openapi.yml,\n  openapi/opsgenie-schedule-openapi.yml, openapi/opsgenie-service-openapi.yml, openapi/opsgenie-team-openapi.yml,\n  openapi/opsgenie-user-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: genieKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication using the GenieKey scheme.\n  sources:\n  - openapi/opsgenie-account-openapi.yml\n  - openapi/opsgenie-alert-openapi.yml\n  - openapi/opsgenie-escalation-openapi.yml\n  - openapi/opsgenie-heartbeat-openapi.yml\n  - openapi/opsgenie-incident-openapi.yml\n  - openapi/opsgenie-integration-openapi.yml\n\
  \  - openapi/opsgenie-maintenance-openapi.yml\n  - openapi/opsgenie-notification-rule-openapi.yml\n  - openapi/opsgenie-schedule-openapi.yml\n  - openapi/opsgenie-service-openapi.yml\n  - openapi/opsgenie-team-openapi.yml\n  - openapi/opsgenie-user-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/authentication/opsgenie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alerts
- Incident Management
- Monitoring
- On-Call
---
