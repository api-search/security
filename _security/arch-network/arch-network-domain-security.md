---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arch.network
  spf: true
hosts:
- cert_expires: Sep 29 22:09:45 2026 GMT
  host: arch.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arch Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arch Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Arch Network
provider_slug: arch-network
slug: arch-network-domain-security
source_filename: arch-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arch.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:09:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arch.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch-network/refs/heads/main/security/arch-network-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Web3
- Bitcoin
- Blockchain
- DeFi
- Smart Contracts
- JSON-RPC
- Web3 SDK
---
