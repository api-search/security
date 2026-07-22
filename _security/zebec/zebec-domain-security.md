---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zebec.io
  spf: true
hosts:
- cert_expires: Aug 31 21:15:56 2026 GMT
  host: docs.zebec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 05:57:25 2026 GMT
  host: api.zebec.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zebec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zebec, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zebec
provider_slug: zebec
slug: zebec-domain-security
source_filename: zebec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.zebec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:15:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zebec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 05:57:25 2026 GMT\n  hsts: false\ndomains:\n- domain: zebec.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zebec/refs/heads/main/security/zebec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payroll
- Blockchain
- Cryptocurrency
- Streaming Payments
- Web3
- DeFi
- SDKs
- Stablecoins
- Solana
- Cards
---
