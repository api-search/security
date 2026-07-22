---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: 01.xyz
  spf: false
hosts:
- cert_expires: Aug 21 11:25:30 2026 GMT
  host: 01.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 01 Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 01 Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: 01 Exchange
provider_slug: 01-exchange
slug: 01-exchange-domain-security
source_filename: 01-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 01.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:25:30 2026 GMT\n  hsts: null\ndomains:\n- domain: 01.xyz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/01-exchange/refs/heads/main/security/01-exchange-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Crypto Web3
- Decentralized Finance
- Solana
- Derivatives
- Perpetual Futures
- Decentralized Exchange
- Blockchain
---
