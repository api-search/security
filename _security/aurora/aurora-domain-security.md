---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aurora.dev
  spf: true
hosts:
- cert_expires: Jan  8 11:49:54 2027 GMT
  host: aurora.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 22:38:03 2026 GMT
  host: doc.aurora.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 21:59:13 2026 GMT
  host: mainnet.aurora.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aurora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurora, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aurora
provider_slug: aurora
slug: aurora-domain-security
source_filename: aurora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurora.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 11:49:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: doc.aurora.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 22:38:03 2026 GMT\n  hsts: false\n- host: mainnet.aurora.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:59:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aurora.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora/refs/heads/main/security/aurora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- EVM
- Web3
- JSON-RPC
- NEAR
- Ethereum
- Layer 2
- Smart Contracts
- DeFi
---
