---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: darwinbox.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: darwinbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  2 06:02:36 2026 GMT
  host: api-docs.darwinbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 17:13:52 2026 GMT
  host: api.darwinbox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Darwinbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Darwinbox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Darwinbox
provider_slug: darwinbox
slug: darwinbox-domain-security
source_filename: darwinbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: darwinbox.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.darwinbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:02:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.darwinbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:13:52 2026 GMT\n  hsts: null\ndomains:\n- domain: darwinbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/darwinbox/refs/heads/main/security/darwinbox-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- HRMS
- HR
- Human Resources
- Payroll
- Recruitment
- Performance Management
- Attendance
- Workforce Analytics
- Enterprise
- HCM
---
