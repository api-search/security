---
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
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan  5 19:53:18 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Monitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Monitor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
slug: microsoft-azure-monitor-domain-security
source_filename: microsoft-azure-monitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/security/microsoft-azure-monitor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
---
