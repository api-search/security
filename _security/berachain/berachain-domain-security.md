---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: berachain.com
  spf: true
hosts:
- cert_expires: Aug 24 14:51:29 2026 GMT
  host: www.berachain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 07:51:15 2026 GMT
  host: docs.berachain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 09:03:28 2026 GMT
  host: rpc.berachain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Berachain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Berachain, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Berachain
provider_slug: berachain
slug: berachain-domain-security
source_filename: berachain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.berachain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:51:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.berachain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 07:51:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.berachain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 09:03:28 2026 GMT\n  hsts: null\ndomains:\n- domain: berachain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/berachain/refs/heads/main/security/berachain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Layer 1
- EVM
- Proof of Liquidity
- DeFi
- JSON-RPC
- BeaconKit
---
