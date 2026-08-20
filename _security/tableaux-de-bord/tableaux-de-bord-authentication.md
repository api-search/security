---
api_key_in:
- header
api_specs:
- filename: tableaux-de-bord-alerting-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Alerting API
  slug: tableaux-de-bord-alerting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-alerting-api-openapi.yml
- filename: tableaux-de-bord-annotations-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Annotations API
  slug: tableaux-de-bord-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-annotations-api-openapi.yml
- filename: tableaux-de-bord-dashboards-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Dashboards API
  slug: tableaux-de-bord-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-dashboards-api-openapi.yml
- filename: tableaux-de-bord-datasources-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Datasources API
  slug: tableaux-de-bord-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-datasources-api-openapi.yml
- filename: tableaux-de-bord-folders-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Folders API
  slug: tableaux-de-bord-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-folders-api-openapi.yml
- filename: tableaux-de-bord-organizations-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Organizations API
  slug: tableaux-de-bord-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-organizations-api-openapi.yml
- filename: tableaux-de-bord-teams-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Teams API
  slug: tableaux-de-bord-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-teams-api-openapi.yml
- filename: tableaux-de-bord-users-api-openapi.yml
  format: yaml
  label: Tableaux De Bord Users API
  slug: tableaux-de-bord-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/tableaux-de-bord-users-api-openapi.yml
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
- METABASE
---
