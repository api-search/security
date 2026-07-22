---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: deblock.com
  spf: true
hosts:
- cert_expires: Sep  2 03:18:50 2026 GMT
  host: deblock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deblock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deblock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Deblock
provider_slug: deblock
slug: deblock-domain-security
source_filename: deblock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deblock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:18:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deblock.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deblock/refs/heads/main/security/deblock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Banking
- Neobank
- Cryptocurrency
- Digital Wallet
- Self-Custody
- Payments
- Visa Card
- IBAN
- Exchange
---
