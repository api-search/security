---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alpenlabs.io
  spf: true
hosts:
- cert_expires: Oct 12 21:32:57 2026 GMT
  host: docs.alpenlabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 07:36:35 2026 GMT
  host: rpc.testnet.alpenlabs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpen Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpen Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alpen Labs
provider_slug: alpen-labs
slug: alpen-labs-domain-security
source_filename: alpen-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.alpenlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc.testnet.alpenlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:36:35 2026 GMT\n  hsts: null\ndomains:\n- domain: alpenlabs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpen-labs/refs/heads/main/security/alpen-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Bitcoin
- Blockchain
- Rollup
- Zero-Knowledge
- EVM
- JSON-RPC
- Web3
- Smart Contracts
---
