---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: picpay.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.picpay.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: developers-business.picpay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PicPay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PicPay
provider_slug: picpay
slug: picpay-domain-security
source_filename: picpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.picpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers-business.picpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: picpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picpay/refs/heads/main/security/picpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Digital Wallet
- Digital Bank
- Neobank
- Fintech
- PIX
- Ecommerce
- Checkout
- Credit Card
- Loans
- Investments
- Insurance
- Brazil
- Latin America
- Super App
---
