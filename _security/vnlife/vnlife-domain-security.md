---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vnpay.vn
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vnpayment.vn
  spf: false
hosts:
- cert_expires: Jan 13 10:11:02 2027 GMT
  host: vnpay.vn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: sandbox.vnpayment.vn
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vnlife Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VNLIFE, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VNLIFE
provider_slug: vnlife
slug: vnlife-domain-security
source_filename: vnlife-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vnpay.vn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 10:11:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.vnpayment.vn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vnpay.vn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vnpayment.vn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vnlife/refs/heads/main/security/vnlife-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Payment Gateway
- QR Payments
- E-Commerce
- Vietnam
- Financial Services
---
