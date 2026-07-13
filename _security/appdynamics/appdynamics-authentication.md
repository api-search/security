---
api_key_in:
- header
api_specs:
- filename: appdynamics-controller-rest-api-openapi.yml
  format: yaml
  label: AppDynamics Controller REST API
  slug: controller-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-controller-rest-api-openapi.yml
- filename: appdynamics-metric-and-snapshot-api-openapi.yml
  format: yaml
  label: AppDynamics Metric and Snapshot API
  slug: metric-and-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-metric-and-snapshot-api-openapi.yml
- filename: appdynamics-alert-and-respond-api-openapi.yml
  format: yaml
  label: AppDynamics Alert and Respond API
  slug: alert-and-respond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-alert-and-respond-api-openapi.yml
- filename: appdynamics-configuration-api-openapi.yml
  format: yaml
  label: AppDynamics Configuration API
  slug: configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-configuration-api-openapi.yml
- filename: appdynamics-analytics-events-api-openapi.yml
  format: yaml
  label: AppDynamics Analytics Events API
  slug: analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-analytics-events-api-openapi.yml
- filename: appdynamics-database-agent-api-openapi.yml
  format: yaml
  label: AppDynamics Database Agent API
  slug: database-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-database-agent-api-openapi.yml
- filename: appdynamics-machine-agent-api-openapi.yml
  format: yaml
  label: AppDynamics Machine Agent API
  slug: machine-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-machine-agent-api-openapi.yml
- filename: appdynamics-cloud-observability-api-openapi.yml
  format: yaml
  label: Cisco Cloud Observability API
  slug: cloud-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-cloud-observability-api-openapi.yml
- filename: appdynamics-authentication-api-openapi.yml
  format: yaml
  label: AppDynamics OAuth Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-authentication-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appdynamics Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppDynamics secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppDynamics
provider_slug: appdynamics
scheme_count: 3
schemes:
- description: OAuth 2.0 access token obtained from the /controller/api/oauth/access_token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appdynamics-alert-and-respond-api-openapi.yml
  - openapi/appdynamics-cloud-observability-api-openapi.yml
  - openapi/appdynamics-configuration-api-openapi.yml
  - openapi/appdynamics-controller-rest-api-openapi.yml
  - openapi/appdynamics-database-agent-api-openapi.yml
  - openapi/appdynamics-metric-and-snapshot-api-openapi.yml
  type: http
- description: HTTP Basic authentication using user@account:password format.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/appdynamics-alert-and-respond-api-openapi.yml
  - openapi/appdynamics-configuration-api-openapi.yml
  - openapi/appdynamics-controller-rest-api-openapi.yml
  - openapi/appdynamics-database-agent-api-openapi.yml
  - openapi/appdynamics-metric-and-snapshot-api-openapi.yml
  type: http
- description: The API key for authenticating with the Events Service. Provided alongside the X-Events-API-AccountName header.
  in: header
  name: apiKey
  parameter: X-Events-API-Key
  sources:
  - openapi/appdynamics-analytics-events-api-openapi.yml
  type: apiKey
slug: appdynamics-authentication
source_filename: appdynamics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appdynamics-alert-and-respond-api-openapi.yml, openapi/appdynamics-analytics-events-api-openapi.yml,\n  openapi/appdynamics-cloud-observability-api-openapi.yml, openapi/appdynamics-configuration-api-openapi.yml,\n  openapi/appdynamics-controller-rest-api-openapi.yml, openapi/appdynamics-database-agent-api-openapi.yml,\n  openapi/appdynamics-metric-and-snapshot-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained from the /controller/api/oauth/access_token endpoint.\n  sources:\n  - openapi/appdynamics-alert-and-respond-api-openapi.yml\n  - openapi/appdynamics-cloud-observability-api-openapi.yml\n  - openapi/appdynamics-configuration-api-openapi.yml\n  - openapi/appdynamics-controller-rest-api-openapi.yml\n  - openapi/appdynamics-database-agent-api-openapi.yml\n  - openapi/appdynamics-metric-and-snapshot-api-openapi.yml\n\
  - name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using user@account:password format.\n  sources:\n  - openapi/appdynamics-alert-and-respond-api-openapi.yml\n  - openapi/appdynamics-configuration-api-openapi.yml\n  - openapi/appdynamics-controller-rest-api-openapi.yml\n  - openapi/appdynamics-database-agent-api-openapi.yml\n  - openapi/appdynamics-metric-and-snapshot-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Events-API-Key\n  description: The API key for authenticating with the Events Service. Provided alongside the\n    X-Events-API-AccountName header.\n  sources:\n  - openapi/appdynamics-analytics-events-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/authentication/appdynamics-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
---
