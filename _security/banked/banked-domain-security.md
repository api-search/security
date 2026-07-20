---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: banked.com
  spf: true
hosts:
- cert_expires: Sep 13 16:16:40 2026 GMT
  host: banked.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 06:21:24 2026 GMT
  host: developer.banked.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api.banked.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banked, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Banked
provider_slug: banked
slug: banked-domain-security
source_filename: banked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: banked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.banked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:21:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.banked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: banked.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banked/refs/heads/main/security/banked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Open Banking
- Account-to-Account
- Pay by Bank
- Fintech
- Payment Processing
- Payouts
---
