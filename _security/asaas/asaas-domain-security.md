---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asaas.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.asaas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:15:52 2026 GMT
  host: docs.asaas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.asaas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asaas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asaas, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asaas
provider_slug: asaas
slug: asaas-domain-security
source_filename: asaas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n- host: docs.asaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:15:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.asaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: asaas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asaas/refs/heads/main/security/asaas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Billing
- Subscriptions
- Pix
- Boleto
- Credit Card
- Checkout
- Split Payments
- Webhooks
- Digital Account
- Receivables
- Invoicing
- Brazil
- Fintech
- SMB
---
