---
api_specs:
- filename: loki-openapi.yml
  format: yaml
  label: Loki HTTP API
  slug: loki-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loki/refs/heads/main/openapi/loki-openapi.yml
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
name: Loki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Loki
provider_slug: loki
slug: loki-domain-security
source_filename: loki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grafana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grafana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loki/refs/heads/main/security/loki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logging
- Observability
- Open Source
- Grafana
---
