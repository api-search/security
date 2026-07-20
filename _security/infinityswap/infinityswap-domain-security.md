---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: bitfinity.network
  spf: true
hosts:
- cert_expires: Aug 17 14:30:20 2026 GMT
  host: bitfinity.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 00:11:04 2026 GMT
  host: docs.bitfinity.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:10:17 2026 GMT
  host: mainnet.bitfinity.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infinityswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InfinitySwap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: InfinitySwap
provider_slug: infinityswap
slug: infinityswap-domain-security
source_filename: infinityswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitfinity.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 14:30:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bitfinity.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mainnet.bitfinity.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:10:17 2026 GMT\n  hsts: null\ndomains:\n- domain: bitfinity.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinityswap/refs/heads/main/security/infinityswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Defi
- Blockchain
- Ethereum
- EVM
- Bitcoin
- Layer 2
- Internet Computer
- Smart Contracts
- JSON-RPC
- Web3
- Cryptocurrency
---
