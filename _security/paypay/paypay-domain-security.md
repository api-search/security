---
api_specs:
- filename: paypay-opa-openapi-original.json
  format: json
  label: PayPay Open Payment API (OPA v2)
  slug: paypay-open-payment-api-opa-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypay/refs/heads/main/openapi/paypay-opa-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ne.jp
  spf: false
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: apigw.paypay.ne.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: apigw.stg.paypay.ne.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: apigw.sandbox.paypay.ne.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paypay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayPay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PayPay
provider_slug: paypay
slug: paypay-domain-security
source_filename: paypay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apigw.paypay.ne.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\n- host: apigw.stg.paypay.ne.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\n- host: apigw.sandbox.paypay.ne.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ne.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypay/refs/heads/main/security/paypay-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Payments
- Mobile Payments
- QR Code Payments
- Digital Wallet
- Japan
- Merchant Payments
---
