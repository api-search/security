---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: citcon.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: citconpay.com
  spf: true
hosts:
- cert_expires: Oct 10 23:41:51 2026 GMT
  host: citcon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 03:42:01 2026 GMT
  host: www.citcon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 09:10:42 2026 GMT
  host: api.citconpay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Citcon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citcon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Citcon
provider_slug: citcon
slug: citcon-domain-security
source_filename: citcon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citcon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:41:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.citcon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:42:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.citconpay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 09:10:42 2026 GMT\n  hsts: null\ndomains:\n- domain: citcon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: citconpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citcon/refs/heads/main/security/citcon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Cross-Border Payments
- Digital Wallets
- Payment Gateway
- BNPL
- Global Payouts
- Fintech
---
