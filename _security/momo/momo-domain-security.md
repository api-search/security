---
api_specs:
- filename: postman.yaml
  format: yaml
  label: MoMo All-in-One Payment Gateway (AIO v2)
  slug: aio-payment-gateway
  spec_type: Postman
  url: https://developers.momo.vn/v3/docs/payment/api/other/postman/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: momo.vn
  spf: true
hosts:
- cert_expires: Nov  8 13:11:56 2026 GMT
  host: www.momo.vn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 07:27:13 2027 GMT
  host: developers.momo.vn
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 07:27:13 2027 GMT
  host: payment.momo.vn
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Momo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoMo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MoMo
provider_slug: momo
slug: momo-domain-security
source_filename: momo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.momo.vn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 13:11:56 2026 GMT\n  hsts: false\n- host: developers.momo.vn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 07:27:13 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: payment.momo.vn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 07:27:13 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: momo.vn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momo/refs/heads/main/security/momo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Mobile Payments
- FinTech
- Digital Wallet
- Payment Gateway
- QR Payments
- Disbursement
- Buy Now Pay Later
- E-commerce
- Vietnam
---
