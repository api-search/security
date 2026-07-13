---
api_specs:
- filename: prometheus-server-api-openapi.yml
  format: yaml
  label: Prometheus Server HTTP API
  slug: prometheus-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-server-api-openapi.yml
- filename: prometheus-alertmanager-api-openapi.yml
  format: yaml
  label: Prometheus Alertmanager API v2
  slug: prometheus-alertmanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-alertmanager-api-openapi.yml
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
name: Prometheus Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prometheus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prometheus
provider_slug: prometheus-io
slug: prometheus-io-domain-security
source_filename: prometheus-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prometheus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:23:26 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: prometheus.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/security/prometheus-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Monitoring
- Metrics
- Observability
- Time Series
- Alerting
- Cloud Native
- CNCF
- Open Source
- PromQL
- Telemetry
---
