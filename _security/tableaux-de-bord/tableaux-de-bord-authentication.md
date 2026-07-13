---
api_key_in:
- header
api_specs:
- filename: grafana-dashboard-openapi.yml
  format: yaml
  label: Grafana HTTP API
  slug: grafana
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/grafana-dashboard-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tableaux De Bord Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tableaux De Bord secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tableaux De Bord
provider_slug: tableaux-de-bord
scheme_count: 2
schemes:
- description: Basic auth with Grafana username and password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/grafana-dashboard-openapi.yml
  type: http
- description: API key authentication using 'Bearer {api-key}'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/grafana-dashboard-openapi.yml
  type: apiKey
slug: tableaux-de-bord-authentication
source_filename: tableaux-de-bord-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grafana-dashboard-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic auth with Grafana username and password\n  sources:\n  - openapi/grafana-dashboard-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication using 'Bearer {api-key}'\n  sources:\n  - openapi/grafana-dashboard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/authentication/tableaux-de-bord-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Dashboards
- Business Intelligence
- Analytics
- Data Visualization
- Monitoring
- Grafana
- Metabase
---
