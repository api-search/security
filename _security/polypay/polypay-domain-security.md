---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: polypay.com
  spf: true
hosts:
- cert_expires: Dec 31 21:46:10 2026 GMT
  host: polypay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PolyPay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolyPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PolyPay
provider_slug: polypay
slug: polypay-domain-security
source_filename: polypay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polypay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 21:46:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: polypay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/polypay/security/polypay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Payments
- Merchant Processing
- Payment Terminals
- Virtual Terminals
- Mobile Payments
- Point‑of‑Sale Systems
- Integration
---
