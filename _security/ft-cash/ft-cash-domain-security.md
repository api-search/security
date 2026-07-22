---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ftcash.com
  spf: false
hosts:
- cert_expires: Mar  8 08:44:11 2027 GMT
  host: ftcash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ft Cash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FT Cash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: FT Cash
provider_slug: ft-cash
slug: ft-cash-domain-security
source_filename: ft-cash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ftcash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 08:44:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ftcash.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ft-cash/refs/heads/main/security/ft-cash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Payments
- Lending
- SME
- Financial Inclusion
- India
---
