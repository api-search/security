---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kakaopay.com
  spf: false
hosts:
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: www.kakaopay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: developers.kakaopay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: open-api.kakaopay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kakaopay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KakaoPay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KakaoPay
provider_slug: kakaopay
slug: kakaopay-domain-security
source_filename: kakaopay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kakaopay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.kakaopay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-api.kakaopay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kakaopay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakaopay/refs/heads/main/security/kakaopay-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Payments
- Mobile Payments
- QR Code Payments
- Subscription Billing
- Money Transfer
- Fintech
- Korean
- REST API
---
