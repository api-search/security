---
api_key_in:
- header
api_specs:
- filename: new-relic-openapi.yml
  format: yaml
  label: New Relic REST API v2
  slug: new-relic-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-openapi.yml
- filename: new-relic-metric-api-openapi.yml
  format: yaml
  label: New Relic Metric API
  slug: new-relic-metric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-metric-api-openapi.yml
- filename: new-relic-event-api-openapi.yml
  format: yaml
  label: New Relic Event API
  slug: new-relic-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-event-api-openapi.yml
- filename: new-relic-log-api-openapi.yml
  format: yaml
  label: New Relic Log API
  slug: new-relic-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-log-api-openapi.yml
- filename: new-relic-trace-api-openapi.yml
  format: yaml
  label: New Relic Trace API
  slug: new-relic-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/openapi/new-relic-trace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: New Relic Authentication
name_suffix: Authentication
oauth_flows: []
overview: New Relic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: New Relic
provider_slug: new-relic
scheme_count: 1
schemes:
- description: New Relic License Key or Ingest API Key
  in: header
  name: apiKey
  parameter: Api-Key
  sources:
  - openapi/new-relic-event-api-openapi.yml
  - openapi/new-relic-log-api-openapi.yml
  - openapi/new-relic-metric-api-openapi.yml
  - openapi/new-relic-openapi.yml
  - openapi/new-relic-trace-api-openapi.yml
  type: apiKey
slug: new-relic-authentication
source_filename: new-relic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/new-relic-event-api-openapi.yml, openapi/new-relic-log-api-openapi.yml, openapi/new-relic-metric-api-openapi.yml,\n  openapi/new-relic-openapi.yml, openapi/new-relic-trace-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: New Relic License Key or Ingest API Key\n  sources:\n  - openapi/new-relic-event-api-openapi.yml\n  - openapi/new-relic-log-api-openapi.yml\n  - openapi/new-relic-metric-api-openapi.yml\n  - openapi/new-relic-openapi.yml\n  - openapi/new-relic-trace-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/authentication/new-relic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
---
