---
api_key_in:
- header
api_specs:
- filename: checkly-accounts-api-openapi.yml
  format: yaml
  label: Checkly Accounts API
  slug: checkly-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-accounts-api-openapi.yml
- filename: checkly-alert-channels-api-openapi.yml
  format: yaml
  label: Checkly Alert Channels API
  slug: checkly-alert-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-alert-channels-api-openapi.yml
- filename: checkly-analytics-api-openapi.yml
  format: yaml
  label: Checkly Analytics API
  slug: checkly-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-analytics-api-openapi.yml
- filename: checkly-check-alerts-api-openapi.yml
  format: yaml
  label: Checkly Check Alerts API
  slug: checkly-check-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-alerts-api-openapi.yml
- filename: checkly-check-groups-api-openapi.yml
  format: yaml
  label: Checkly Check Groups API
  slug: checkly-check-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-groups-api-openapi.yml
- filename: checkly-check-results-api-openapi.yml
  format: yaml
  label: Checkly Check Results API
  slug: checkly-check-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-results-api-openapi.yml
- filename: checkly-check-statuses-api-openapi.yml
  format: yaml
  label: Checkly Check Statuses API
  slug: checkly-check-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-statuses-api-openapi.yml
- filename: checkly-checks-api-openapi.yml
  format: yaml
  label: Checkly Checks API
  slug: checkly-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-checks-api-openapi.yml
- filename: checkly-dashboards-api-openapi.yml
  format: yaml
  label: Checkly Dashboards API
  slug: checkly-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-dashboards-api-openapi.yml
- filename: checkly-heartbeats-api-openapi.yml
  format: yaml
  label: Checkly Heartbeats API
  slug: checkly-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-heartbeats-api-openapi.yml
- filename: checkly-incidents-api-openapi.yml
  format: yaml
  label: Checkly Incidents API
  slug: checkly-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-incidents-api-openapi.yml
- filename: checkly-locations-api-openapi.yml
  format: yaml
  label: Checkly Locations API
  slug: checkly-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-locations-api-openapi.yml
- filename: checkly-maintenance-windows-api-openapi.yml
  format: yaml
  label: Checkly Maintenance Windows API
  slug: checkly-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-maintenance-windows-api-openapi.yml
- filename: checkly-private-locations-api-openapi.yml
  format: yaml
  label: Checkly Private Locations API
  slug: checkly-private-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-private-locations-api-openapi.yml
- filename: checkly-reports-api-openapi.yml
  format: yaml
  label: Checkly Reports API
  slug: checkly-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-reports-api-openapi.yml
- filename: checkly-variables-api-openapi.yml
  format: yaml
  label: Checkly Variables API
  slug: checkly-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-variables-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Checkly
provider_slug: checkly
scheme_count: 2
schemes:
- description: API Key authentication for Checkly API. You can get your API key at https://app.checklyhq.com/settings/user/api-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/checkly-openapi.json
  type: http
- description: Your Checkly account ID. You can find it at https://app.checklyhq.com/settings/account/general
  in: header
  name: accountId
  parameter: X-Checkly-Account
  sources:
  - openapi/checkly-openapi.json
  type: apiKey
slug: checkly-authentication
source_filename: checkly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkly-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API Key authentication for Checkly API. You can get your API key at https://app.checklyhq.com/settings/user/api-keys\n  sources:\n  - openapi/checkly-openapi.json\n- name: accountId\n  type: apiKey\n  in: header\n  parameter: X-Checkly-Account\n  description: Your Checkly account ID. You can find it at https://app.checklyhq.com/settings/account/general\n  sources:\n  - openapi/checkly-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/authentication/checkly-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Monitoring
- Testing
---
