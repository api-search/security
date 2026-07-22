---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: enosys.global
  spf: true
hosts:
- cert_expires: Sep 11 03:57:09 2026 GMT
  host: enosys.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enosys Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enosys Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Enosys Markets
provider_slug: enosys-markets
slug: enosys-markets-domain-security
source_filename: enosys-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enosys.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:57:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: enosys.global\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enosys-markets/refs/heads/main/security/enosys-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- DeFi
- Blockchain
- Decentralized Exchange
- Flare Network
- Smart Contracts
- Cryptocurrency
- Web3
- Lending
---
