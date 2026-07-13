---
api_key_in:
- header
api_specs:
- filename: metrics_API.json
  format: json
  label: Azure Monitor Metrics API
  slug: azure-monitor-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2023-10-01/metrics_API.json
- filename: metricDefinitions_API.json
  format: json
  label: Azure Monitor Metric Definitions API
  slug: azure-monitor-metric-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2023-10-01/metricDefinitions_API.json
- filename: azure-monitor-metrics-batch-openapi.yml
  format: yaml
  label: Azure Monitor Metrics Batch API
  slug: azure-monitor-metrics-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/openapi/azure-monitor-metrics-batch-openapi.yml
- filename: OperationalInsights.json
  format: json
  label: Azure Monitor Logs API
  slug: azure-monitor-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/operationalinsights/data-plane/Microsoft.OperationalInsights/stable/2022-10-27/OperationalInsights.json
- filename: azure-monitor-logs-ingestion-openapi.yml
  format: yaml
  label: Azure Monitor Logs Ingestion API
  slug: azure-monitor-logs-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/openapi/azure-monitor-logs-ingestion-openapi.yml
- filename: alertRules_API.json
  format: json
  label: Azure Monitor Alerts API
  slug: azure-monitor-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2016-03-01/alertRules_API.json
- filename: scheduledQueryRule_API.json
  format: json
  label: Azure Monitor Scheduled Query Rules API
  slug: azure-monitor-scheduled-query-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2021-08-01/scheduledQueryRule_API.json
- filename: actionGroups_API.json
  format: json
  label: Azure Monitor Action Groups API
  slug: azure-monitor-action-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2022-06-01/actionGroups_API.json
- filename: autoscale_API.json
  format: json
  label: Azure Monitor Autoscale API
  slug: azure-monitor-autoscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2022-10-01/autoscale_API.json
- filename: AppInsights.json
  format: json
  label: Azure Application Insights API
  slug: azure-application-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/applicationinsights/data-plane/Microsoft.Insights/stable/v1/AppInsights.json
- filename: diagnosticsSettings_API.json
  format: json
  label: Azure Monitor Diagnostic Settings API
  slug: azure-monitor-diagnostic-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2021-05-01-preview/diagnosticsSettings_API.json
- filename: activityLogs_API.json
  format: json
  label: Azure Monitor Activity Log API
  slug: azure-monitor-activity-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2015-04-01/activityLogs_API.json
- filename: dataCollectionRules_API.json
  format: json
  label: Azure Monitor Data Collection Rules API
  slug: azure-monitor-data-collection-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2023-03-11/dataCollectionRules_API.json
- filename: dataCollectionEndpoints_API.json
  format: json
  label: Azure Monitor Data Collection Endpoints API
  slug: azure-monitor-data-collection-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/monitor/resource-manager/Microsoft.Insights/stable/2023-03-11/dataCollectionEndpoints_API.json
- filename: azure-monitor-private-link-scopes-openapi.yml
  format: yaml
  label: Azure Monitor Private Link Scopes API
  slug: azure-monitor-private-link-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/openapi/azure-monitor-private-link-scopes-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Monitor Authentication
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/authentication/microsoft-azure-monitor-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
---
