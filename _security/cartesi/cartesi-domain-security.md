---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cartesi.io
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: cartesi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cartesi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartesi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cartesi
provider_slug: cartesi
slug: cartesi-domain-security
source_filename: cartesi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartesi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cartesi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartesi/refs/heads/main/security/cartesi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Layer 2
- Optimistic Rollups
- Ethereum
- EVM
- RISC-V
- Linux
- Virtual Machine
- Cartesi Machine
- Rollups
- Fraud Proofs
- DAVE
- Smart Contracts
- Decentralized Applications
- Web3
- Open Source
---
