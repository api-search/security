---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yieldprotocol.com
  spf: true
hosts:
- cert_expires: Aug 21 09:53:50 2026 GMT
  host: yieldprotocol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yield Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yield Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yield Protocol
provider_slug: yield-protocol
slug: yield-protocol-domain-security
source_filename: yield-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yieldprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:53:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yieldprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yield-protocol/refs/heads/main/security/yield-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Defi
- DeFi
- Ethereum
- Lending
- Fixed Rate
- Smart Contracts
- Solidity
---
