---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: aellaapp.com
  spf: false
hosts:
- cert_expires: Oct 15 04:22:37 2026 GMT
  host: aellaapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:53:15 2026 GMT
  host: api.aellaapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aella Credit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aella Credit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Aella Credit
provider_slug: aella-credit
slug: aella-credit-domain-security
source_filename: aella-credit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aellaapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:22:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.aellaapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aellaapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aella-credit/refs/heads/main/security/aella-credit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Fintech
- Banking
- Microfinance
- Payments
- Lending
- Digital Wallet
- KYC
- Identity Verification
- Direct Debit
- Nigeria
- Africa
- Fintech as a Service
---
