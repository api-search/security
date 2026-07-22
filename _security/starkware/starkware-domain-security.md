---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: starkware.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starknet.io
  spf: true
hosts:
- cert_expires: Oct 10 03:13:17 2026 GMT
  host: starkware.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 18:05:29 2026 GMT
  host: docs.starknet.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 04:17:45 2026 GMT
  host: docs.starkware.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starkware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starkware, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Starkware
provider_slug: starkware
slug: starkware-domain-security
source_filename: starkware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: starkware.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.starknet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:05:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.starkware.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 04:17:45 2026 GMT\n  hsts: false\ndomains:\n- domain: starkware.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: starknet.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starkware/refs/heads/main/security/starkware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Ethereum
- Layer 2
- ZK-Rollup
- Zero-Knowledge Proofs
- JSON-RPC
- Cryptography
- Cairo
- Web3
- Scaling
- Starknet
---
