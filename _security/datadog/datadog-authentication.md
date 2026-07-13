---
api_key_in:
- header
api_specs:
- filename: datadog-api-openapi.yml
  format: yaml
  label: Datadog API
  slug: datadog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-api-openapi.yml
- filename: datadog-metrics-openapi.yml
  format: yaml
  label: Datadog Metrics API
  slug: datadog-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-metrics-openapi.yml
- filename: datadog-logs-openapi.yml
  format: yaml
  label: Datadog Logs API
  slug: datadog-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-logs-openapi.yml
- filename: datadog-events-openapi.yml
  format: yaml
  label: Datadog Events API
  slug: datadog-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-events-openapi.yml
- filename: datadog-monitors-openapi.yml
  format: yaml
  label: Datadog Monitors API
  slug: datadog-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-monitors-openapi.yml
- filename: datadog-incidents-openapi.yml
  format: yaml
  label: Datadog Incidents API
  slug: datadog-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-incidents-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Datadog Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Datadog secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Datadog
provider_slug: datadog
scheme_count: 4
schemes:
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: /oauth2/v1/authorize
    flow: authorizationCode
    scopes: 68
    tokenUrl: /oauth2/v1/token
  name: AuthZ
  sources:
  - openapi/datadog-api-openapi.yml
  type: oauth2
- description: Your Datadog API Key.
  in: header
  name: apiKeyAuth
  parameter: DD-API-KEY
  sources:
  - openapi/datadog-api-openapi.yml
  - openapi/datadog-events-openapi.yml
  - openapi/datadog-incidents-openapi.yml
  - openapi/datadog-logs-openapi.yml
  - openapi/datadog-metrics-openapi.yml
  - openapi/datadog-monitors-openapi.yml
  type: apiKey
- description: Your Datadog APP Key.
  in: header
  name: appKeyAuth
  parameter: DD-APPLICATION-KEY
  sources:
  - openapi/datadog-api-openapi.yml
  - openapi/datadog-incidents-openapi.yml
  - openapi/datadog-monitors-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datadog-api-openapi.yml
  type: http
slug: datadog-authentication
source_filename: datadog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datadog-api-openapi.yml, openapi/datadog-events-openapi.yml, openapi/datadog-incidents-openapi.yml,\n  openapi/datadog-logs-openapi.yml, openapi/datadog-metrics-openapi.yml, openapi/datadog-monitors-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: AuthZ\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v1/authorize\n    tokenUrl: /oauth2/v1/token\n    scopes: 68\n  description: This API uses OAuth 2 with the implicit grant flow.\n  sources:\n  - openapi/datadog-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: DD-API-KEY\n  description: Your Datadog API Key.\n  sources:\n  - openapi/datadog-api-openapi.yml\n  - openapi/datadog-events-openapi.yml\n  - openapi/datadog-incidents-openapi.yml\n  - openapi/datadog-logs-openapi.yml\n  - openapi/datadog-metrics-openapi.yml\n\
  \  - openapi/datadog-monitors-openapi.yml\n- name: appKeyAuth\n  type: apiKey\n  in: header\n  parameter: DD-APPLICATION-KEY\n  description: Your Datadog APP Key.\n  sources:\n  - openapi/datadog-api-openapi.yml\n  - openapi/datadog-incidents-openapi.yml\n  - openapi/datadog-monitors-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/datadog-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/authentication/datadog-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
---
