---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: schedex.me
  spf: false
hosts:
- cert_expires: Sep 25 05:27:47 2026 GMT
  host: schedex.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schedex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schedex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Schedex
provider_slug: schedex
slug: schedex-domain-security
source_filename: schedex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: schedex.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:27:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: schedex.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schedex/refs/heads/main/security/schedex-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- Food and Beverage
- Human Resources
- SaaS
---
