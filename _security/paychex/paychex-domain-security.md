---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paychex.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.paychex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 20 06:33:57 2026 GMT
  host: developer.paychex.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paychex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paychex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paychex
provider_slug: paychex
slug: paychex-domain-security
source_filename: paychex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paychex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.paychex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: paychex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paychex/refs/heads/main/security/paychex-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Payroll
- Human Resources
- HR
- Benefits
- Time and Attendance
- Fortune 1000
---
