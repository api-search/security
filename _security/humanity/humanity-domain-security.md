---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humanity.com
  spf: true
hosts:
- cert_expires: Oct  2 20:32:18 2026 GMT
  host: www.humanity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 22:31:15 2026 GMT
  host: platform.humanity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humanity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humanity, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Humanity
provider_slug: humanity
slug: humanity-domain-security
source_filename: humanity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humanity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:32:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.humanity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 22:31:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humanity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanity/refs/heads/main/security/humanity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Management
- Employee Scheduling
- Shift Planning
- Time Tracking
- Human Resources
- Leave Management
- Payroll
- Workforce
---
