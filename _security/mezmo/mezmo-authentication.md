---
api_key_in:
- header
api_specs:
- filename: mezmo-auditevents-api-openapi.yml
  format: yaml
  label: Mezmo AuditEvents API
  slug: mezmo-auditevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-auditevents-api-openapi.yml
- filename: mezmo-classification-api-openapi.yml
  format: yaml
  label: Mezmo Classification API
  slug: mezmo-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-classification-api-openapi.yml
- filename: mezmo-deployments-api-openapi.yml
  format: yaml
  label: Mezmo Deployments API
  slug: mezmo-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-deployments-api-openapi.yml
- filename: mezmo-destinations-api-openapi.yml
  format: yaml
  label: Mezmo Destinations API
  slug: mezmo-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-destinations-api-openapi.yml
- filename: mezmo-edgeclients-api-openapi.yml
  format: yaml
  label: Mezmo EdgeClients API
  slug: mezmo-edgeclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-edgeclients-api-openapi.yml
- filename: mezmo-exclusions-api-openapi.yml
  format: yaml
  label: Mezmo Exclusions API
  slug: mezmo-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-exclusions-api-openapi.yml
- filename: mezmo-export-api-openapi.yml
  format: yaml
  label: Mezmo Export API
  slug: mezmo-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-export-api-openapi.yml
- filename: mezmo-heartbeats-api-openapi.yml
  format: yaml
  label: Mezmo Heartbeats API
  slug: mezmo-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-heartbeats-api-openapi.yml
- filename: mezmo-logs-api-openapi.yml
  format: yaml
  label: Mezmo Logs API
  slug: mezmo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-logs-api-openapi.yml
- filename: mezmo-metrics-api-openapi.yml
  format: yaml
  label: Mezmo Metrics API
  slug: mezmo-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-metrics-api-openapi.yml
- filename: mezmo-pipelines-api-openapi.yml
  format: yaml
  label: Mezmo Pipelines API
  slug: mezmo-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipelines-api-openapi.yml
- filename: mezmo-presetalerts-api-openapi.yml
  format: yaml
  label: Mezmo PresetAlerts API
  slug: mezmo-presetalerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-presetalerts-api-openapi.yml
- filename: mezmo-processors-api-openapi.yml
  format: yaml
  label: Mezmo Processors API
  slug: mezmo-processors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-processors-api-openapi.yml
- filename: mezmo-sources-api-openapi.yml
  format: yaml
  label: Mezmo Sources API
  slug: mezmo-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-sources-api-openapi.yml
- filename: mezmo-suspension-api-openapi.yml
  format: yaml
  label: Mezmo Suspension API
  slug: mezmo-suspension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-suspension-api-openapi.yml
- filename: mezmo-tasks-api-openapi.yml
  format: yaml
  label: Mezmo Tasks API
  slug: mezmo-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-tasks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mezmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mezmo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mezmo
provider_slug: mezmo
scheme_count: 2
schemes:
- name: AccessToken
  scheme: bearer
  sources:
  - openapi/mezmo-alerts-api-openapi.yml
  - openapi/mezmo-archiving-api-openapi.yml
  - openapi/mezmo-edge-api-openapi.yml
  - openapi/mezmo-ingestion-control-api-openapi.yml
  - openapi/mezmo-log-export-api-openapi.yml
  - openapi/mezmo-log-ingestion-api-openapi.yml
  - openapi/mezmo-pipeline-api-openapi.yml
  - openapi/mezmo-pipeline-classification-api-openapi.yml
  - openapi/mezmo-usage-api-openapi.yml
  - openapi/mezmo-views-api-openapi.yml
  type: http
- description: Deprecated service key in Authorization header.
  in: header
  name: ServiceKey
  parameter: Authorization
  sources:
  - openapi/mezmo-log-ingestion-api-openapi.yml
  type: apiKey
slug: mezmo-authentication
source_filename: mezmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mezmo-alerts-api-openapi.yml, openapi/mezmo-archiving-api-openapi.yml, openapi/mezmo-edge-api-openapi.yml,\n  openapi/mezmo-ingestion-control-api-openapi.yml, openapi/mezmo-log-export-api-openapi.yml,\n  openapi/mezmo-log-ingestion-api-openapi.yml, openapi/mezmo-pipeline-api-openapi.yml, openapi/mezmo-pipeline-classification-api-openapi.yml,\n  openapi/mezmo-usage-api-openapi.yml, openapi/mezmo-views-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mezmo-alerts-api-openapi.yml\n  - openapi/mezmo-archiving-api-openapi.yml\n  - openapi/mezmo-edge-api-openapi.yml\n  - openapi/mezmo-ingestion-control-api-openapi.yml\n  - openapi/mezmo-log-export-api-openapi.yml\n  - openapi/mezmo-log-ingestion-api-openapi.yml\n  - openapi/mezmo-pipeline-api-openapi.yml\n  - openapi/mezmo-pipeline-classification-api-openapi.yml\n\
  \  - openapi/mezmo-usage-api-openapi.yml\n  - openapi/mezmo-views-api-openapi.yml\n- name: ServiceKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Deprecated service key in Authorization header.\n  sources:\n  - openapi/mezmo-log-ingestion-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/authentication/mezmo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Observability
- Logs
- Telemetry
- Telemetry Pipeline
- Log Management
- Artificial Intelligence
- SRE
- OpenTelemetry
- DevOps
---
