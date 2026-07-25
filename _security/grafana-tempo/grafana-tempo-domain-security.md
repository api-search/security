---
api_specs:
- filename: grafana-tempo-echo-api-openapi.yml
  format: yaml
  label: Grafana Tempo Echo API
  slug: grafana-tempo-echo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/openapi/grafana-tempo-echo-api-openapi.yml
- filename: grafana-tempo-metrics-api-openapi.yml
  format: yaml
  label: Grafana Tempo Metrics API
  slug: grafana-tempo-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/openapi/grafana-tempo-metrics-api-openapi.yml
- filename: grafana-tempo-ready-api-openapi.yml
  format: yaml
  label: Grafana Tempo Ready API
  slug: grafana-tempo-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/openapi/grafana-tempo-ready-api-openapi.yml
- filename: grafana-tempo-search-api-openapi.yml
  format: yaml
  label: Grafana Tempo Search API
  slug: grafana-tempo-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/openapi/grafana-tempo-search-api-openapi.yml
- filename: grafana-tempo-status-api-openapi.yml
  format: yaml
  label: Grafana Tempo Status API
  slug: grafana-tempo-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/openapi/grafana-tempo-status-api-openapi.yml
- filename: grafana-tempo-traces-api-openapi.yml
  format: yaml
  label: Grafana Tempo Traces API
  slug: grafana-tempo-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/openapi/grafana-tempo-traces-api-openapi.yml
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
name: Grafana Tempo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grafana Tempo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Grafana Tempo
provider_slug: grafana-tempo
slug: grafana-tempo-domain-security
source_filename: grafana-tempo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grafana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grafana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafana-tempo/refs/heads/main/security/grafana-tempo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distributed Tracing
- Grafana
- Microservices
- Observability
- Open Source
---
