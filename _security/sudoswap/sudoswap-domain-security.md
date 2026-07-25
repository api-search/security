---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sudoswap.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: etherscan.io
  spf: true
hosts:
- cert_expires: Sep  5 04:29:46 2026 GMT
  host: sudoswap.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 04:29:46 2026 GMT
  host: docs.sudoswap.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:43:38 2026 GMT
  host: etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sudoswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sudoswap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sudoswap
provider_slug: sudoswap
slug: sudoswap-domain-security
source_filename: sudoswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sudoswap.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:29:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sudoswap.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:29:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:43:38 2026 GMT\n  hsts: false\ndomains:\n- domain: sudoswap.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: etherscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sudoswap/refs/heads/main/security/sudoswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- AMM
- DeFi
- Liquidity
- Bonding Curves
- ERC-721
- ERC-1155
- Ethereum
---
