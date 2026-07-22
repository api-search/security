---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: khazna.app
  spf: true
hosts:
- cert_expires: Oct 11 08:48:49 2026 GMT
  host: khazna.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Khazna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Khazna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Khazna
provider_slug: khazna
slug: khazna-domain-security
source_filename: khazna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: khazna.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 08:48:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: khazna.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/khazna/refs/heads/main/security/khazna-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Financial Services
- Financial Inclusion
- Earned Wage Access
- Payments
- Bill Payments
- Lending
- Savings
- Egypt
- Mobile App
---
