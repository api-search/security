---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yourpay.co
  spf: true
hosts:
- cert_expires: Oct 11 05:00:49 2026 GMT
  host: yourpay.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yourpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YourPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: YourPay
provider_slug: yourpay
slug: yourpay-domain-security
source_filename: yourpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yourpay.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yourpay.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourpay/refs/heads/main/security/yourpay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Payments
- Remittances
- Money Transfer
- Bill Payment
- QRIS
- Indonesia
- Mobile Payments
---
