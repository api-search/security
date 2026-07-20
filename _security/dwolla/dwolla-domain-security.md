---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dwolla.com
  spf: true
hosts:
- cert_expires: Sep 12 20:23:10 2026 GMT
  host: dwolla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 21:51:35 2026 GMT
  host: developers.dwolla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:40:51 2026 GMT
  host: api.dwolla.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dwolla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dwolla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dwolla
provider_slug: dwolla
slug: dwolla-domain-security
source_filename: dwolla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dwolla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:23:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.dwolla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:51:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dwolla.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 20:40:51 2026 GMT\n  hsts: null\ndomains:\n- domain: dwolla.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/security/dwolla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- ACH
- Bank Transfers
- Fintech
- Account-to-Account Payments
- Money Movement
- Instant Payments
- Open Banking
- Webhooks
- KYC
---
