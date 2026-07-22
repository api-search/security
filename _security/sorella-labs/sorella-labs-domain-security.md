---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sorellalabs.xyz
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: angstrom.xyz
  spf: false
hosts:
- cert_expires: Sep 12 01:29:02 2026 GMT
  host: sorellalabs.xyz
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 17 17:43:20 2026 GMT
  host: docs.angstrom.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:01:55 2026 GMT
  host: mainnet.node-lb.angstrom.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sorella Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sorella Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sorella Labs
provider_slug: sorella-labs
slug: sorella-labs-domain-security
source_filename: sorella-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sorellalabs.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 12 01:29:02 2026 GMT\n  hsts: false\n- host: docs.angstrom.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 17:43:20 2026 GMT\n  hsts: false\n- host: mainnet.node-lb.angstrom.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:01:55 2026 GMT\n  hsts: null\ndomains:\n- domain: sorellalabs.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: angstrom.xyz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorella-labs/refs/heads/main/security/sorella-labs-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Crypto Infrastructure
- DeFi
- Decentralized Exchange
- MEV
- Ethereum
- Uniswap V4
- JSON-RPC
- Blockchain
- Trading
---
