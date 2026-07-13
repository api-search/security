---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: astropay.com
  spf: true
hosts:
- cert_expires: Oct  1 04:26:17 2026 GMT
  host: www.astropay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: developers.astropay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astropay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AstroPay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AstroPay
provider_slug: astropay
slug: astropay-domain-security
source_filename: astropay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astropay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.astropay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: astropay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astropay/refs/heads/main/security/astropay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Payouts
- Wallet
- Digital Wallet
- Multicurrency
- Cards
- Card Issuing
- PIX
- LATAM
- Latin America
- Brazil
- Argentina
- Mexico
- Chile
- Peru
- Colombia
- Uruguay
- Fintech
- Foreign Exchange
- Cross-Border Payments
- Checkout
- QR Payments
- Tokenization
- Embedded Finance
- Money Transfer
- Remittance
- Gaming Payments
- Marketplace Payments
- Payroll
---
