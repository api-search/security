---
api_specs:
- filename: carbone-openapi.yml
  format: yaml
  label: Carbone Cloud HTTP API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbone/refs/heads/main/openapi/carbone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carbone.io
  spf: true
hosts:
- cert_expires: Sep 22 10:02:39 2026 GMT
  host: carbone.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  2 20:18:36 2026 GMT
  host: api.carbone.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carbone
provider_slug: carbone
slug: carbone-domain-security
source_filename: carbone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:02:39 2026 GMT\n  hsts: false\n- host: api.carbone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 20:18:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carbone.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbone/refs/heads/main/security/carbone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Generation
- PDF
- Templates
- Open Source
- Office
- DOCX
- XLSX
---
