---
api_specs:
- filename: prometheus-admin-api-openapi.yml
  format: yaml
  label: Prometheus Admin API
  slug: prometheus-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-admin-api-openapi.yml
- filename: prometheus-alerts-api-openapi.yml
  format: yaml
  label: Prometheus Alerts API
  slug: prometheus-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-alerts-api-openapi.yml
- filename: prometheus-lifecycle-api-openapi.yml
  format: yaml
  label: Prometheus Lifecycle API
  slug: prometheus-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-lifecycle-api-openapi.yml
- filename: prometheus-metadata-api-openapi.yml
  format: yaml
  label: Prometheus Metadata API
  slug: prometheus-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-metadata-api-openapi.yml
- filename: prometheus-metrics-api-openapi.yml
  format: yaml
  label: Prometheus Metrics API
  slug: prometheus-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-metrics-api-openapi.yml
- filename: prometheus-query-api-openapi.yml
  format: yaml
  label: Prometheus Query API
  slug: prometheus-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-query-api-openapi.yml
- filename: prometheus-receivers-api-openapi.yml
  format: yaml
  label: Prometheus Receivers API
  slug: prometheus-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-receivers-api-openapi.yml
- filename: prometheus-rules-api-openapi.yml
  format: yaml
  label: Prometheus Rules API
  slug: prometheus-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-rules-api-openapi.yml
- filename: prometheus-silences-api-openapi.yml
  format: yaml
  label: Prometheus Silences API
  slug: prometheus-silences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-silences-api-openapi.yml
- filename: prometheus-status-api-openapi.yml
  format: yaml
  label: Prometheus Status API
  slug: prometheus-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-status-api-openapi.yml
- filename: prometheus-targets-api-openapi.yml
  format: yaml
  label: Prometheus Targets API
  slug: prometheus-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-targets-api-openapi.yml
- filename: prometheus-tsdb-api-openapi.yml
  format: yaml
  label: Prometheus TSDB API
  slug: prometheus-tsdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/openapi/prometheus-tsdb-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: prometheus.io
  spf: false
hosts:
- cert_expires: Sep  1 15:23:26 2026 GMT
  host: prometheus.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prometheus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prometheus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prometheus
provider_slug: prometheus
slug: prometheus-domain-security
source_filename: prometheus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prometheus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:23:26 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: prometheus.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometheus/refs/heads/main/security/prometheus-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Alerting
- Metrics
- Monitoring
- Observability
- Time Series
---
