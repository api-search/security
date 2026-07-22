---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mystenlabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sui.io
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: mystenlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 11:46:41 2026 GMT
  host: docs.sui.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 14:09:56 2026 GMT
  host: fullnode.mainnet.sui.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mysten Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mysten Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mysten Labs
provider_slug: mysten-labs
slug: mysten-labs-domain-security
source_filename: mysten-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mystenlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sui.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:46:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: fullnode.mainnet.sui.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:09:56 2026 GMT\n  hsts: null\ndomains:\n- domain: mystenlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sui.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mysten-labs/refs/heads/main/security/mysten-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Web3
- Sui
- Move
- JSON-RPC
- GraphQL
- gRPC
- SDK
- Smart Contracts
- Decentralized Storage
- Cryptocurrency
---
