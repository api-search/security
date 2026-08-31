---
api_specs:
- filename: moogsoft-alerts-incidents-openapi.yaml
  format: yaml
  label: Moogsoft Alerts/Incidents API
  slug: alerts-incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-alerts-incidents-openapi.yaml
- filename: moogsoft-azure-service-openapi.yaml
  format: yaml
  label: Moogsoft Azure Application Insights API
  slug: azure-app-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-azure-service-openapi.yaml
- filename: moogsoft-byo-api-service-openapi.yaml
  format: yaml
  label: Moogsoft Create Your Own Integration API
  slug: create-your-own-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-byo-api-service-openapi.yaml
- filename: moogsoft-cloudwatch-service-openapi.yaml
  format: yaml
  label: Moogsoft Amazon CloudWatch API
  slug: cloudwatch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-cloudwatch-service-openapi.yaml
- filename: moogsoft-collectors-openapi.yaml
  format: yaml
  label: Moogsoft Collector V2 API
  slug: collector
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-collectors-openapi.yaml
- filename: moogsoft-config-openapi.yaml
  format: yaml
  label: Moogsoft Config API
  slug: config
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-config-openapi.yaml
- filename: moogsoft-events-integration-openapi.yaml
  format: yaml
  label: Moogsoft Events Integration API
  slug: events-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-events-integration-openapi.yaml
- filename: moogsoft-incident-responder-openapi.yaml
  format: yaml
  label: Moogsoft On-Call API
  slug: on-call
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-incident-responder-openapi.yaml
- filename: moogsoft-metric-processor-openapi.yaml
  format: yaml
  label: Moogsoft Rollup Service API
  slug: rollup-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-metric-processor-openapi.yaml
- filename: moogsoft-metrics-integration-openapi.yaml
  format: yaml
  label: Moogsoft Metrics API
  slug: metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-metrics-integration-openapi.yaml
- filename: moogsoft-pagerduty-service-openapi.yaml
  format: yaml
  label: Moogsoft PagerDuty Integration API
  slug: pagerduty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-pagerduty-service-openapi.yaml
- filename: moogsoft-probable-rootcause-openapi.yaml
  format: yaml
  label: Moogsoft Probable Root Cause API
  slug: probable-root-cause
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-probable-rootcause-openapi.yaml
- filename: moogsoft-similar-incidents-openapi.yaml
  format: yaml
  label: Moogsoft Similar Incidents API
  slug: similar-incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-similar-incidents-openapi.yaml
- filename: moogsoft-ui-services-openapi.yaml
  format: yaml
  label: Moogsoft UI Services API
  slug: ui-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-ui-services-openapi.yaml
- filename: moogsoft-user-management-openapi.yaml
  format: yaml
  label: Moogsoft User Management API
  slug: user-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-user-management-openapi.yaml
- filename: moogsoft-webhook-service-v2-openapi.yaml
  format: yaml
  label: Moogsoft Webhook API
  slug: webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-webhook-service-v2-openapi.yaml
- filename: moogsoft-workflow-engine-service-openapi.yaml
  format: yaml
  label: Moogsoft Workflow Engine API
  slug: workflow-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/openapi/moogsoft-workflow-engine-service-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moogsoft.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moogsoft.ai
  spf: true
hosts:
- cert_expires: Nov 23 12:02:57 2026 GMT
  host: www.moogsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 07:32:58 2026 GMT
  host: api.docs.moogsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 11:23:00 2026 GMT
  host: api.moogsoft.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moogsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moogsoft, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Moogsoft
provider_slug: moogsoft
slug: moogsoft-domain-security
source_filename: moogsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moogsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 12:02:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.docs.moogsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 07:32:58 2026 GMT\n  hsts: null\n- host: api.moogsoft.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 11:23:00 2026 GMT\n  hsts: null\ndomains:\n- domain: moogsoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: moogsoft.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moogsoft/refs/heads/main/security/moogsoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Incident Management
- Observability
- Alerting
- Event Management
- Anomaly Detection
- Correlation
- On-Call
- Monitoring
- IT Operations
- DevOps
- SRE
---
