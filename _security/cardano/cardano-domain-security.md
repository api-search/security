---
api_specs:
- filename: blockfrost-cardano-api-openapi.yml
  format: yaml
  label: Blockfrost Cardano API
  slug: blockfrost-cardano-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardano/refs/heads/main/openapi/blockfrost-cardano-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blockfrost.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockfrost.io
  spf: true
hosts:
- cert_expires: Sep 30 02:45:09 2026 GMT
  host: blockfrost.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:17:05 2026 GMT
  host: cardano-mainnet.blockfrost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:04:48 2026 GMT
  host: ipfs.blockfrost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardano, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cardano
provider_slug: cardano
slug: cardano-domain-security
source_filename: cardano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockfrost.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:45:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cardano-mainnet.blockfrost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ipfs.blockfrost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:04:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blockfrost.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: blockfrost.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardano/refs/heads/main/security/cardano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Cryptocurrency
- Proof-of-Stake
- Smart Contracts
- Web3
---
