---
api_key_in:
- header
api_specs:
- filename: opsgenie-alert-openapi.yml
  format: yaml
  label: OpsGenie Alert API
  slug: opsgenie-alert
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-alert-openapi.yml
- filename: opsgenie-incident-openapi.yml
  format: yaml
  label: OpsGenie Incident API
  slug: opsgenie-incident
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-incident-openapi.yml
- filename: opsgenie-user-openapi.yml
  format: yaml
  label: OpsGenie User API
  slug: opsgenie-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-user-openapi.yml
- filename: opsgenie-team-openapi.yml
  format: yaml
  label: OpsGenie Team API
  slug: opsgenie-team
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-team-openapi.yml
- filename: opsgenie-schedule-openapi.yml
  format: yaml
  label: OpsGenie Schedule API
  slug: opsgenie-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-schedule-openapi.yml
- filename: opsgenie-escalation-openapi.yml
  format: yaml
  label: OpsGenie Escalation API
  slug: opsgenie-escalation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-escalation-openapi.yml
- filename: opsgenie-integration-openapi.yml
  format: yaml
  label: OpsGenie Integration API
  slug: opsgenie-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-integration-openapi.yml
- filename: opsgenie-heartbeat-openapi.yml
  format: yaml
  label: OpsGenie Heartbeat API
  slug: opsgenie-heartbeat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-heartbeat-openapi.yml
- filename: opsgenie-service-openapi.yml
  format: yaml
  label: OpsGenie Service API
  slug: opsgenie-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-service-openapi.yml
- filename: opsgenie-notification-rule-openapi.yml
  format: yaml
  label: OpsGenie Notification Rule API
  slug: opsgenie-notification-rule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-notification-rule-openapi.yml
- filename: opsgenie-account-openapi.yml
  format: yaml
  label: OpsGenie Account API
  slug: opsgenie-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-account-openapi.yml
- filename: opsgenie-maintenance-openapi.yml
  format: yaml
  label: OpsGenie Maintenance API
  slug: opsgenie-maintenance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsgenie/refs/heads/main/openapi/opsgenie-maintenance-openapi.yml
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
- Operations
---
