---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: payengine.co
  spf: true
hosts:
- cert_expires: Nov 13 22:11:44 2026 GMT
  host: www.payengine.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 08:33:49 2026 GMT
  host: docs.payengine.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 02:45:16 2026 GMT
  host: api.payengine.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayEngine, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PayEngine
provider_slug: payengine
slug: payengine-domain-security
source_filename: payengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payengine.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 22:11:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.payengine.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 08:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.payengine.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:45:16 2026 GMT\n  hsts: null\ndomains:\n- domain: payengine.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payengine/refs/heads/main/security/payengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Embedded Payments
- Payment Facilitation
- Merchant Onboarding
- Payment Gateway
- Financial Services
- ACH
- Tokenization
- Webhooks
- Fintech
- Company
---
