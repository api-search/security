---
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
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
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
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure Monitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Monitor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
slug: microsoft-azure-monitor-domain-security
source_filename: microsoft-azure-monitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-monitor/security/microsoft-azure-monitor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
---
