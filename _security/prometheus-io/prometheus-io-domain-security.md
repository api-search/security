---
api_specs:
- filename: prometheus-io-admin-api-openapi.yml
  format: yaml
  label: Prometheus Admin API
  slug: prometheus-io-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-admin-api-openapi.yml
- filename: prometheus-io-alert-api-openapi.yml
  format: yaml
  label: Prometheus Alert API
  slug: prometheus-io-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-alert-api-openapi.yml
- filename: prometheus-io-alertgroup-api-openapi.yml
  format: yaml
  label: Prometheus Alertgroup API
  slug: prometheus-io-alertgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-alertgroup-api-openapi.yml
- filename: prometheus-io-alerts-api-openapi.yml
  format: yaml
  label: Prometheus Alerts API
  slug: prometheus-io-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-alerts-api-openapi.yml
- filename: prometheus-io-features-api-openapi.yml
  format: yaml
  label: Prometheus Features API
  slug: prometheus-io-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-features-api-openapi.yml
- filename: prometheus-io-general-api-openapi.yml
  format: yaml
  label: Prometheus General API
  slug: prometheus-io-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-general-api-openapi.yml
- filename: prometheus-io-labels-api-openapi.yml
  format: yaml
  label: Prometheus Labels API
  slug: prometheus-io-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-labels-api-openapi.yml
- filename: prometheus-io-metadata-api-openapi.yml
  format: yaml
  label: Prometheus Metadata API
  slug: prometheus-io-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-metadata-api-openapi.yml
- filename: prometheus-io-notifications-api-openapi.yml
  format: yaml
  label: Prometheus Notifications API
  slug: prometheus-io-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-notifications-api-openapi.yml
- filename: prometheus-io-otlp-api-openapi.yml
  format: yaml
  label: Prometheus Otlp API
  slug: prometheus-io-otlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-otlp-api-openapi.yml
- filename: prometheus-io-query-api-openapi.yml
  format: yaml
  label: Prometheus Query API
  slug: prometheus-io-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-query-api-openapi.yml
- filename: prometheus-io-receiver-api-openapi.yml
  format: yaml
  label: Prometheus Receiver API
  slug: prometheus-io-receiver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-receiver-api-openapi.yml
- filename: prometheus-io-remote-api-openapi.yml
  format: yaml
  label: Prometheus Remote API
  slug: prometheus-io-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-remote-api-openapi.yml
- filename: prometheus-io-rules-api-openapi.yml
  format: yaml
  label: Prometheus Rules API
  slug: prometheus-io-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-rules-api-openapi.yml
- filename: prometheus-io-series-api-openapi.yml
  format: yaml
  label: Prometheus Series API
  slug: prometheus-io-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-series-api-openapi.yml
- filename: prometheus-io-silence-api-openapi.yml
  format: yaml
  label: Prometheus Silence API
  slug: prometheus-io-silence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-silence-api-openapi.yml
- filename: prometheus-io-status-api-openapi.yml
  format: yaml
  label: Prometheus Status API
  slug: prometheus-io-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-status-api-openapi.yml
- filename: prometheus-io-targets-api-openapi.yml
  format: yaml
  label: Prometheus Targets API
  slug: prometheus-io-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometheus-io/refs/heads/main/openapi/prometheus-io-targets-api-openapi.yml
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
hosts_probed: 1
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
- Prometheus
- Monitoring
- Metrics
- Observability
- Time Series
- Alerting
- Cloud-Native
- CNCF
- Open Source
- PromQL
- Telemetry
---
