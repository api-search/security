---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: billie.io
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: www.billie.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 12 15:12:04 2026 GMT
  host: docs.billie.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: paella.billie.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Billie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billie, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Billie
provider_slug: billie
slug: billie-domain-security
source_filename: billie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.billie.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.billie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: paella.billie.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: billie.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/security/billie-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- BNPL
- Buy Now Pay Later
- B2B
- Invoicing
- Checkout
- Germany
---
