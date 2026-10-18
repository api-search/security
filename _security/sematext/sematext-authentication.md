---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: sematext-alert-notifications-api-openapi.yml
  format: yaml
  label: Sematext Alert Notifications API
  slug: sematext-alert-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-alert-notifications-api-openapi.yml
- filename: sematext-alerts-api-openapi.yml
  format: yaml
  label: Sematext Alerts API
  slug: sematext-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-alerts-api-openapi.yml
- filename: sematext-app-guests-api-openapi.yml
  format: yaml
  label: Sematext App guests API
  slug: sematext-app-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-guests-api-openapi.yml
- filename: sematext-app-ips-api-openapi.yml
  format: yaml
  label: Sematext App IPs API
  slug: sematext-app-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-ips-api-openapi.yml
- filename: sematext-app-tokens-api-openapi.yml
  format: yaml
  label: Sematext App tokens API
  slug: sematext-app-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-tokens-api-openapi.yml
- filename: sematext-apps-api-openapi.yml
  format: yaml
  label: Sematext Apps API
  slug: sematext-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-apps-api-openapi.yml
- filename: sematext-billing-api-openapi.yml
  format: yaml
  label: Sematext Billing API
  slug: sematext-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-billing-api-openapi.yml
- filename: sematext-experience-app-api-openapi.yml
  format: yaml
  label: Sematext Experience App API
  slug: sematext-experience-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-experience-app-api-openapi.yml
- filename: sematext-logs-app-api-openapi.yml
  format: yaml
  label: Sematext Logs App API
  slug: sematext-logs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-logs-app-api-openapi.yml
- filename: sematext-logs-app-usage-api-openapi.yml
  format: yaml
  label: Sematext Logs App usage API
  slug: sematext-logs-app-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-logs-app-usage-api-openapi.yml
- filename: sematext-monitoring-app-api-openapi.yml
  format: yaml
  label: Sematext Monitoring App API
  slug: sematext-monitoring-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-monitoring-app-api-openapi.yml
- filename: sematext-notifications-api-openapi.yml
  format: yaml
  label: Sematext Notifications API
  slug: sematext-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-notifications-api-openapi.yml
- filename: sematext-reset-password-api-openapi.yml
  format: yaml
  label: Sematext Reset Password API
  slug: sematext-reset-password-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-reset-password-api-openapi.yml
- filename: sematext-subscriptions-api-openapi.yml
  format: yaml
  label: Sematext Subscriptions API
  slug: sematext-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-subscriptions-api-openapi.yml
- filename: sematext-tags-api-openapi.yml
  format: yaml
  label: Sematext Tags API
  slug: sematext-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sematext Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sematext secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sematext
provider_slug: sematext
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/sematext-cloud-openapi-original.json
  - openapi/sematext-openapi.yml
  type: apiKey
slug: sematext-authentication
source_filename: sematext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/sematext-cloud-openapi-original.json, openapi/sematext-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/sematext-cloud-openapi-original.json\n  - openapi/sematext-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/authentication/sematext-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Observability
- Monitoring
- Logging
- Log Management
- Elasticsearch
- Tracing
- Synthetic Monitoring
- OpenTelemetry
---
