---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ubeya.com
  spf: true
hosts:
- cert_expires: Oct  2 23:40:47 2026 GMT
  host: ubeya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubeya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubeya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ubeya
provider_slug: ubeya
slug: ubeya-domain-security
source_filename: ubeya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubeya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:40:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ubeya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubeya/refs/heads/main/security/ubeya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Management
- Staffing
- Scheduling
- Time and Attendance
- Payroll
- Events
- Hospitality
- Human Resources
---
