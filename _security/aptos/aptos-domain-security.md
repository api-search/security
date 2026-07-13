---
api_specs:
- filename: spec.yaml
  format: yaml
  label: Aptos Fullnode REST API
  slug: fullnode-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/aptos-labs/aptos-core/main/api/doc/spec.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: aptos.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aptoslabs.com
  spf: true
hosts:
- cert_expires: Oct  9 05:19:18 2026 GMT
  host: aptos.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:05:08 2026 GMT
  host: api.mainnet.aptoslabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:05:08 2026 GMT
  host: grpc.mainnet.aptoslabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aptos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aptos, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Aptos
provider_slug: aptos
slug: aptos-domain-security
source_filename: aptos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aptos.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:19:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mainnet.aptoslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:05:08 2026 GMT\n  hsts: null\n- host: grpc.mainnet.aptoslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:05:08 2026 GMT\n  hsts: null\ndomains:\n- domain: aptos.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: aptoslabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptos/refs/heads/main/security/aptos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- Move
- Layer 1
- Cryptocurrency
- NFT
- Smart Contracts
- DeFi
- Transactions
- Accounts
- GraphQL
- gRPC
---
