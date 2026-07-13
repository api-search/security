---
api_specs:
- filename: 7shifts-openapi.yml
  format: yaml
  label: 7shifts REST API v2
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/openapi/7shifts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 7shifts.com
  spf: true
hosts:
- cert_expires: Sep  4 15:14:31 2026 GMT
  host: www.7shifts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 21:05:25 2026 GMT
  host: developers.7shifts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 15:14:31 2026 GMT
  host: api.7shifts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 7Shifts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7shifts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 7shifts
provider_slug: 7shifts
slug: 7shifts-domain-security
source_filename: 7shifts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.7shifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:14:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.7shifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 21:05:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.7shifts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:14:31 2026 GMT\n  hsts: null\ndomains:\n- domain: 7shifts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7shifts/refs/heads/main/security/7shifts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaurant
- Scheduling
- Workforce Management
- Employee Scheduling
- Time Tracking
- HRIS
- Labor
---
