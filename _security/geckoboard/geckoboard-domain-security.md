---
api_specs:
- filename: geckoboard-openapi.yml
  format: yaml
  label: Geckoboard Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geckoboard/refs/heads/main/openapi/geckoboard-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geckoboard.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.geckoboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: developer.geckoboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.geckoboard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geckoboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geckoboard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Geckoboard
provider_slug: geckoboard
slug: geckoboard-domain-security
source_filename: geckoboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geckoboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: developer.geckoboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: api.geckoboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: geckoboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geckoboard/refs/heads/main/security/geckoboard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dashboards
- Data Visualization
- Business Intelligence
- KPI Tracking
- Real-Time Reporting
- TV Dashboards
---
