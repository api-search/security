---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cronitor-groups-api-openapi.yml
  format: yaml
  label: Cronitor Groups API
  slug: cronitor-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-groups-api-openapi.yml
- filename: cronitor-notifications-api-openapi.yml
  format: yaml
  label: Cronitor Notifications API
  slug: cronitor-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-notifications-api-openapi.yml
- filename: cronitor-aggregates-api-openapi.yml
  format: yaml
  label: Cronitor Aggregates API
  slug: cronitor-aggregates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-aggregates-api-openapi.yml
- filename: cronitor-environments-api-openapi.yml
  format: yaml
  label: Cronitor Environments API
  slug: cronitor-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-environments-api-openapi.yml
- filename: cronitor-integrations-api-openapi.yml
  format: yaml
  label: Cronitor Integrations API
  slug: cronitor-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-integrations-api-openapi.yml
- filename: cronitor-issues-api-openapi.yml
  format: yaml
  label: Cronitor Issues API
  slug: cronitor-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-issues-api-openapi.yml
- filename: cronitor-keys-api-openapi.yml
  format: yaml
  label: Cronitor Keys API
  slug: cronitor-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-keys-api-openapi.yml
- filename: cronitor-maintenance-windows-api-openapi.yml
  format: yaml
  label: Cronitor Maintenance Windows API
  slug: cronitor-maintenance-windows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-maintenance-windows-api-openapi.yml
- filename: cronitor-metrics-api-openapi.yml
  format: yaml
  label: Cronitor Metrics API
  slug: cronitor-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-metrics-api-openapi.yml
- filename: cronitor-monitors-api-openapi.yml
  format: yaml
  label: Cronitor Monitors API
  slug: cronitor-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-monitors-api-openapi.yml
- filename: cronitor-search-api-openapi.yml
  format: yaml
  label: Cronitor Search API
  slug: cronitor-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-search-api-openapi.yml
- filename: cronitor-site-errors-api-openapi.yml
  format: yaml
  label: Cronitor Site Errors API
  slug: cronitor-site-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-site-errors-api-openapi.yml
- filename: cronitor-sites-api-openapi.yml
  format: yaml
  label: Cronitor Sites API
  slug: cronitor-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-sites-api-openapi.yml
- filename: cronitor-statuspage-components-api-openapi.yml
  format: yaml
  label: Cronitor Statuspage Components API
  slug: cronitor-statuspage-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-statuspage-components-api-openapi.yml
- filename: cronitor-statuspages-api-openapi.yml
  format: yaml
  label: Cronitor Statuspages API
  slug: cronitor-statuspages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-statuspages-api-openapi.yml
- filename: cronitor-telemetry-api-openapi.yml
  format: yaml
  label: Cronitor Telemetry API
  slug: cronitor-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-telemetry-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cronitor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cronitor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cronitor
provider_slug: cronitor
scheme_count: 1
schemes:
- description: Use your Cronitor API key as the username; leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cronitor-groups-notifications-api-openapi.yml
  - openapi/cronitor-monitors-api-openapi.yml
  type: http
slug: cronitor-authentication
source_filename: cronitor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cronitor-groups-notifications-api-openapi.yml, openapi/cronitor-monitors-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your Cronitor API key as the username; leave the password blank.\n  sources:\n  - openapi/cronitor-groups-notifications-api-openapi.yml\n  - openapi/cronitor-monitors-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cronitor/authentication/cronitor-authentication.yml
summary_line: http · 1 scheme
tags:
- Monitoring
- Cron Jobs
- Scheduled Tasks
- Alerting
- Uptime
- Telemetry
- Status Pages
- Scheduling
---
