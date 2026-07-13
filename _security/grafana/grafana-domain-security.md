---
api_specs:
- filename: grafana-api.yml
  format: yaml
  label: Grafana HTTP API
  slug: grafana-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana/refs/heads/main/openapi/grafana-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grafana.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: grafana.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grafana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grafana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Grafana
provider_slug: grafana
slug: grafana-domain-security
source_filename: grafana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grafana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grafana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafana/refs/heads/main/security/grafana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alerting
- Analytics
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
- Traces
- Visualization
---
