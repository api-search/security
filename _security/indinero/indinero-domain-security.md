---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: indinero.com
  spf: true
hosts:
- cert_expires: Sep  3 10:52:36 2026 GMT
  host: indinero.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indinero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indinero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Indinero
provider_slug: indinero
slug: indinero-domain-security
source_filename: indinero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indinero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:52:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: indinero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indinero/refs/heads/main/security/indinero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounting
- Bookkeeping
- Tax
- CFO Services
- Payroll
- Finance as a Service
- Fintech
- Small Business
---
