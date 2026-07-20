---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boku.com
  spf: true
hosts:
- cert_expires: Sep 30 13:15:55 2026 GMT
  host: www.boku.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: developer.boku.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boku, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boku
provider_slug: boku
slug: boku-domain-security
source_filename: boku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.boku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boku/refs/heads/main/security/boku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Mobile Payments
- Carrier Billing
- Digital Wallets
- Local Payment Methods
- Subscriptions
- Fintech
---
