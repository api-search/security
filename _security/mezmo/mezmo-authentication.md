---
api_key_in:
- header
api_specs:
- filename: mezmo-log-ingestion-api-openapi.yml
  format: yaml
  label: Mezmo Log Ingestion API
  slug: mezmo-log-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-log-ingestion-api-openapi.yml
- filename: mezmo-log-export-api-openapi.yml
  format: yaml
  label: Mezmo Log Export API
  slug: mezmo-log-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-log-export-api-openapi.yml
- filename: mezmo-views-api-openapi.yml
  format: yaml
  label: Mezmo Views API
  slug: mezmo-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-views-api-openapi.yml
- filename: mezmo-alerts-api-openapi.yml
  format: yaml
  label: Mezmo Alerts API
  slug: mezmo-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-alerts-api-openapi.yml
- filename: mezmo-archiving-api-openapi.yml
  format: yaml
  label: Mezmo Archiving API
  slug: mezmo-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-archiving-api-openapi.yml
- filename: mezmo-ingestion-control-api-openapi.yml
  format: yaml
  label: Mezmo Ingestion Control API
  slug: mezmo-ingestion-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-ingestion-control-api-openapi.yml
- filename: mezmo-usage-api-openapi.yml
  format: yaml
  label: Mezmo Usage API
  slug: mezmo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-usage-api-openapi.yml
- filename: mezmo-pipeline-api-openapi.yml
  format: yaml
  label: Mezmo Pipeline API
  slug: mezmo-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipeline-api-openapi.yml
- filename: mezmo-pipeline-classification-api-openapi.yml
  format: yaml
  label: Mezmo Pipeline Classification API
  slug: mezmo-pipeline-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipeline-classification-api-openapi.yml
- filename: mezmo-edge-api-openapi.yml
  format: yaml
  label: Mezmo Edge API
  slug: mezmo-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-edge-api-openapi.yml
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
- AI
- SRE
- OpenTelemetry
- DevOps
---
