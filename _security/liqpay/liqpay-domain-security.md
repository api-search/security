---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liqpay.ua
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: www.liqpay.ua
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Liqpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiqPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LiqPay
provider_slug: liqpay
slug: liqpay-domain-security
source_filename: liqpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liqpay.ua\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liqpay.ua\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liqpay/refs/heads/main/security/liqpay-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Payments
- Fintech
- Ukraine
- Cards
- Subscriptions
- Invoicing
- P2P Transfers
- PrivatBank
---
