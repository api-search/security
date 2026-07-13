---
api_specs:
- filename: high-mobility-openapi.yml
  format: yaml
  label: High Mobility Vehicle API
  slug: high-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/openapi/high-mobility-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: high-mobility.com
  spf: true
hosts:
- cert_expires: Sep 29 01:02:51 2026 GMT
  host: high-mobility.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 09:38:59 2026 GMT
  host: api.high-mobility.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:48:20 2026 GMT
  host: sandbox.api.high-mobility.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: High Mobility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for High Mobility, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: High Mobility
provider_slug: high-mobility
slug: high-mobility-domain-security
source_filename: high-mobility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: high-mobility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.high-mobility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 09:38:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.api.high-mobility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:48:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: high-mobility.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/security/high-mobility-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automotive
- Connected Cars
- IoT
- Vehicle Data
---
