---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keep.network
  spf: true
hosts:
- cert_expires: Sep 28 10:47:30 2026 GMT
  host: keep.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keep Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keep Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Keep Network
provider_slug: keep-network
slug: keep-network-domain-security
source_filename: keep-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keep.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:47:30 2026 GMT\n  hsts: null\ndomains:\n- domain: keep.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keep-network/refs/heads/main/security/keep-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blockchain
- Cryptocurrency
- Bitcoin
- Ethereum
- DeFi
- Smart Contracts
- Web3
- Cryptography
- Decentralized Finance
---
