---
api_specs:
- filename: mantle-network-asyncapi.yml
  format: yaml
  label: Mantle WebSocket (Mainnet)
  slug: websocket-mainnet
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mantle-network/refs/heads/main/asyncapi/mantle-network-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mantle.xyz
  spf: true
hosts:
- cert_expires: Sep 19 09:20:56 2026 GMT
  host: www.mantle.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 16:07:42 2026 GMT
  host: docs.mantle.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: rpc.mantle.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mantle Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mantle Network, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mantle Network
provider_slug: mantle-network
slug: mantle-network-domain-security
source_filename: mantle-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mantle.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:20:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mantle.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:07:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc.mantle.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mantle.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mantle-network/refs/heads/main/security/mantle-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Layer 2
- Ethereum
- Rollup
- EigenDA
- Liquid Staking
- JSON-RPC
- Crypto
- Web3
---
