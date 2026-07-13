---
api_key_in:
- header
api_specs:
- filename: grafana-api.yml
  format: yaml
  label: Grafana HTTP API
  slug: grafana-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana/refs/heads/main/openapi/grafana-api.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Grafana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grafana secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Grafana
provider_slug: grafana
scheme_count: 3
schemes:
- description: Service account token or API key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/grafana-api.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/grafana-api.yml
  - openapi/grafana-openapi.yml
  type: http
- description: 'Format: Bearer <api-key>'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/grafana-api.yml
  - openapi/grafana-openapi.yml
  type: apiKey
slug: grafana-authentication
source_filename: grafana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grafana-api.yml, openapi/grafana-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Service account token or API key\n  sources:\n  - openapi/grafana-api.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/grafana-api.yml\n  - openapi/grafana-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format: Bearer <api-key>'\n  sources:\n  - openapi/grafana-api.yml\n  - openapi/grafana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafana/refs/heads/main/authentication/grafana-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Alerting
- Analytics
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
- Traces
- Visualization
---
