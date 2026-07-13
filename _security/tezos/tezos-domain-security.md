---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tzkt.io
  spf: false
hosts:
- cert_expires: Sep 19 03:45:48 2026 GMT
  host: tzkt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:44:00 2026 GMT
  host: api.tzkt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tezos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tezos, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tezos
provider_slug: tezos
slug: tezos-domain-security
source_filename: tezos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tzkt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:45:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tzkt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:44:00 2026 GMT\n  hsts: false\ndomains:\n- domain: tzkt.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tezos/refs/heads/main/security/tezos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Tezos
- Blockchain
- TzKT
- Baking Bad
- Cryptocurrency
- Smart Contracts
- NFT
- Tokens
- Delegations
- Staking
- Governance
- FA1.2
- FA2
- WebSocket
---
