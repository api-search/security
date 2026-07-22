---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pemo.io
  spf: true
hosts:
- cert_expires: Oct 14 07:30:56 2026 GMT
  host: pemo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pemo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pemo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pemo
provider_slug: pemo
slug: pemo-domain-security
source_filename: pemo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pemo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:30:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pemo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pemo/refs/heads/main/security/pemo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- Corporate Cards
- Spend Management
- Expense Management
- Accounting Automation
- Invoice Management
- UAE
- Saudi Arabia
- Payments
---
