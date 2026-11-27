---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-azure-monitor-datacollectionruleconfigurationmetadata-api-openapi.yml
  format: yaml
  label: Azure Monitor Data Collection Rule Configuration Metadata API
  slug: microsoft-azure-monitor-datacollectionruleconfigurationmetadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-monitor/openapi/microsoft-azure-monitor-datacollectionruleconfigurationmetadata-api-openapi.yml
- filename: microsoft-azure-monitor-operations-api-openapi.yml
  format: yaml
  label: Azure Monitor Operations API
  slug: microsoft-azure-monitor-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-monitor/openapi/microsoft-azure-monitor-operations-api-openapi.yml
- filename: microsoft-azure-monitor-scheduledqueryrules-api-openapi.yml
  format: yaml
  label: Azure Monitor Scheduled Query Rules API
  slug: microsoft-azure-monitor-scheduledqueryrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-monitor/openapi/microsoft-azure-monitor-scheduledqueryrules-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Azure Monitor Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Azure Monitor secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/azure-monitor-action-groups-openapi.yml
  - openapi/azure-monitor-activity-log-openapi.yml
  - openapi/azure-monitor-alerts-openapi.yml
  - openapi/azure-monitor-application-insights-openapi.yml
  - openapi/azure-monitor-autoscale-openapi.yml
  - openapi/azure-monitor-data-collection-endpoints-openapi.yml
  - openapi/azure-monitor-data-collection-rules-openapi.yml
  - openapi/azure-monitor-diagnostic-settings-openapi.yml
  - openapi/azure-monitor-logs-ingestion-openapi.yml
  - openapi/azure-monitor-logs-openapi.yml
  - openapi/azure-monitor-metric-definitions-openapi.yml
  - openapi/azure-monitor-metrics-batch-openapi.yml
  - openapi/azure-monitor-metrics-openapi.yml
  - openapi/azure-monitor-private-link-scopes-openapi.yml
  - openapi/azure-monitor-scheduled-query-rules-openapi.yml
  type: oauth2
- description: API key for demo workspace access.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/azure-monitor-application-insights-openapi.yml
  type: apiKey
slug: microsoft-azure-monitor-authentication
source_filename: microsoft-azure-monitor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-monitor-action-groups-openapi.yml, openapi/azure-monitor-activity-log-openapi.yml,\n  openapi/azure-monitor-alerts-openapi.yml, openapi/azure-monitor-application-insights-openapi.yml,\n  openapi/azure-monitor-autoscale-openapi.yml, openapi/azure-monitor-data-collection-endpoints-openapi.yml,\n  openapi/azure-monitor-data-collection-rules-openapi.yml, openapi/azure-monitor-diagnostic-settings-openapi.yml,\n  openapi/azure-monitor-logs-ingestion-openapi.yml, openapi/azure-monitor-logs-openapi.yml,\n  openapi/azure-monitor-metric-definitions-openapi.yml, openapi/azure-monitor-metrics-batch-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  sources:\n  - openapi/azure-monitor-action-groups-openapi.yml\n\
  \  - openapi/azure-monitor-activity-log-openapi.yml\n  - openapi/azure-monitor-alerts-openapi.yml\n  - openapi/azure-monitor-application-insights-openapi.yml\n  - openapi/azure-monitor-autoscale-openapi.yml\n  - openapi/azure-monitor-data-collection-endpoints-openapi.yml\n  - openapi/azure-monitor-data-collection-rules-openapi.yml\n  - openapi/azure-monitor-diagnostic-settings-openapi.yml\n  - openapi/azure-monitor-logs-ingestion-openapi.yml\n  - openapi/azure-monitor-logs-openapi.yml\n  - openapi/azure-monitor-metric-definitions-openapi.yml\n  - openapi/azure-monitor-metrics-batch-openapi.yml\n  - openapi/azure-monitor-metrics-openapi.yml\n  - openapi/azure-monitor-private-link-scopes-openapi.yml\n  - openapi/azure-monitor-scheduled-query-rules-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for demo workspace access.\n  sources:\n  - openapi/azure-monitor-application-insights-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-monitor/authentication/microsoft-azure-monitor-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
---
