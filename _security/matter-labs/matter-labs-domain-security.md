---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: matterlabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zksync.io
  spf: true
hosts:
- cert_expires: Sep 29 10:15:03 2026 GMT
  host: matterlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:47:34 2026 GMT
  host: docs.zksync.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:08:27 2026 GMT
  host: mainnet.era.zksync.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matter Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matter Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Matter Labs
provider_slug: matter-labs
slug: matter-labs-domain-security
source_filename: matter-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matterlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.zksync.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: mainnet.era.zksync.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:08:27 2026 GMT\n  hsts: null\ndomains:\n- domain: matterlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zksync.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matter-labs/refs/heads/main/security/matter-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Ethereum
- Layer 2
- Zero-Knowledge Proofs
- Rollup
- JSON-RPC
- Web3
- Cryptography
- Scaling
---
