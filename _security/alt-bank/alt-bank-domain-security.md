---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: altbank.ai
  spf: true
hosts:
- cert_expires: Aug 19 02:14:55 2026 GMT
  host: altbank.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: developers.altbank.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 02:14:55 2026 GMT
  host: guard.altbank.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alt Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alt Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alt Bank
provider_slug: alt-bank
slug: alt-bank-domain-security
source_filename: alt-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altbank.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:14:55 2026 GMT\n  hsts: false\n- host: developers.altbank.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: guard.altbank.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:14:55 2026 GMT\n  hsts: null\ndomains:\n- domain: altbank.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alt-bank/refs/heads/main/security/alt-bank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Banking
- Credit
- Underwriting
- Credit Cards
- Payments
- KYC
- Risk
- Brazil
- Financial Inclusion
- Banking as a Service
---
