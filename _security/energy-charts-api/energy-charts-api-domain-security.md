---
api_specs:
- filename: energy-charts-api-openapi.yml
  format: yaml
  label: Energy Charts API
  slug: energy-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-charts-api/refs/heads/main/openapi/energy-charts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: energy-charts.info
  spf: true
hosts:
- cert_expires: Oct  5 21:50:37 2026 GMT
  host: www.energy-charts.info
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 21:23:02 2026 GMT
  host: api.energy-charts.info
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Energy Charts Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energy Charts API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Energy Charts API
provider_slug: energy-charts-api
slug: energy-charts-api-domain-security
source_filename: energy-charts-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energy-charts.info\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 21:50:37 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\n- host: api.energy-charts.info\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 21:23:02 2026 GMT\n  hsts: null\ndomains:\n- domain: energy-charts.info\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-charts-api/refs/heads/main/security/energy-charts-api-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Energy
- Electricity
- Renewables
- Grid
- Europe
- Power
- Pricing
- Forecasts
---
