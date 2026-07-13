---
api_specs:
- filename: ukg-ready-openapi.yml
  format: yaml
  label: UKG Ready REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-ready/refs/heads/main/openapi/ukg-ready-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ukg.com
  spf: true
hosts:
- cert_expires: Sep 17 16:56:11 2026 GMT
  host: www.ukg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:39:15 2026 GMT
  host: developer.ukg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ukg Ready Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UKG Ready, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UKG Ready
provider_slug: ukg-ready
slug: ukg-ready-domain-security
source_filename: ukg-ready-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ukg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:56:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ukg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:39:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ukg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukg-ready/refs/heads/main/security/ukg-ready-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HCM
- Human Capital Management
- Payroll
- Workforce Management
- Time and Attendance
- HR
- Benefits
---
