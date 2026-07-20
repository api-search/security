---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gcash.com
  spf: true
hosts:
- cert_expires: Oct 15 11:08:59 2026 GMT
  host: new.gcash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gcash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GCash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GCash
provider_slug: gcash
slug: gcash-domain-security
source_filename: gcash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: new.gcash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:08:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gcash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcash/refs/heads/main/security/gcash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Mobile Wallet
- E-Money
- Fintech
- Digital Payments
- Philippines
- QR Payments
---
