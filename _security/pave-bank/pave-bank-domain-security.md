---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pavebank.com
  spf: true
hosts:
- cert_expires: Sep 28 11:28:49 2026 GMT
  host: pavebank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pave Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pave Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pave Bank
provider_slug: pave-bank
slug: pave-bank-domain-security
source_filename: pave-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pavebank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:28:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pavebank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pave-bank/refs/heads/main/security/pave-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Payments
- Digital Assets
- Stablecoins
- Cross-Border Payments
- Programmable Money
- API
---
