---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sendowl.com
  spf: true
hosts:
- cert_expires: Oct 16 15:28:36 2026 GMT
  host: sendowl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 16:34:56 2026 GMT
  host: dashboard.sendowl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 16:34:56 2026 GMT
  host: api.sendowl.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sendowl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SendOwl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SendOwl
provider_slug: sendowl
slug: sendowl-domain-security
source_filename: sendowl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendowl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:28:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dashboard.sendowl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:34:56 2026 GMT\n  hsts: false\n- host: api.sendowl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:34:56 2026 GMT\n  hsts: null\ndomains:\n- domain: sendowl.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendowl/refs/heads/main/security/sendowl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Commerce
- Digital Products
- Payments
- Subscriptions
- Checkout
- Memberships
- Licensing
- Creator Economy
- Webhooks
---
