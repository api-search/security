---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datadoghq.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.datadoghq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: docs.datadoghq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.datadoghq.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datadog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datadog, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datadog
provider_slug: datadog
slug: datadog-domain-security
source_filename: datadog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datadoghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.datadoghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.datadoghq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datadoghq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/security/datadog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
---
