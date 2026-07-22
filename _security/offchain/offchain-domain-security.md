---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: offchainlabs.com
  spf: true
hosts:
- cert_expires: Oct  8 23:06:22 2026 GMT
  host: www.offchainlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Offchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Offchain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Offchain
provider_slug: offchain
slug: offchain-domain-security
source_filename: offchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.offchainlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:06:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: offchainlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offchain/refs/heads/main/security/offchain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Ethereum
- Layer 2
- Scaling
- Infrastructure
- Web3
- JSON-RPC
- SDK
---
