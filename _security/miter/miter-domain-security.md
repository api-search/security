---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: miter.com
  spf: true
hosts:
- cert_expires: Aug 18 12:56:02 2026 GMT
  host: www.miter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 07:03:37 2026 GMT
  host: api.miter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Miter
provider_slug: miter
slug: miter-domain-security
source_filename: miter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.miter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:56:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.miter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:03:37 2026 GMT\n  hsts: null\ndomains:\n- domain: miter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miter/refs/heads/main/security/miter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Construction
- Payroll
- Human Capital Management
- HR
- Field Operations
- Expense Management
- Workforce Management
- Fintech
---
