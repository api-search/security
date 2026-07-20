---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bka.sh
  spf: false
hosts:
- cert_expires: Oct 16 15:51:14 2026 GMT
  host: developer.bka.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 11:36:37 2026 GMT
  host: tokenized.pay.bka.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bkash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bKash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: bKash
provider_slug: bkash
slug: bkash-domain-security
source_filename: bkash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bka.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:51:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tokenized.pay.bka.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:36:37 2026 GMT\n  hsts: null\ndomains:\n- domain: bka.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bkash/refs/heads/main/security/bkash-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Payments
- Payment Gateway
- Mobile Financial Services
- Digital Wallet
- Bangladesh
- Checkout
- Webhooks
---
