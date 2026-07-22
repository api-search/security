---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stone.com.br
  spf: true
hosts:
- cert_expires: Aug  2 12:30:33 2026 GMT
  host: www.stone.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stone Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stone Co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stone Co
provider_slug: stone-co
slug: stone-co-domain-security
source_filename: stone-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stone.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 12:30:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stone.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stone-co/refs/heads/main/security/stone-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Card Acquiring
- POS
- Point of Sale
- Open Banking
- Banking
- Digital Banking
- PIX
- TED
- Boleto
- Reconciliation
- Subscriptions
- Recurring Billing
- Payment Gateway
- PSP
- 3DS
- Tokenization
- Brazil
- Fintech
- SMB
- Pagar.me
---
