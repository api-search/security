---
api_specs:
- filename: supra-rpc-node-openapi.yml
  format: yaml
  label: Supra RPC Node API
  slug: supra-rpc-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-rpc-node-openapi.yml
- filename: supra-rpc-node-openapi.yml
  format: yaml
  label: Supra Automation API
  slug: supra-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-rpc-node-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: supra.com
  spf: true
hosts:
- cert_expires: Nov 23 18:12:49 2026 GMT
  host: supra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 21:12:04 2026 GMT
  host: docs.supra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 15:18:38 2026 GMT
  host: rpc-mainnet.supra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Supra
provider_slug: supra
slug: supra-domain-security
source_filename: supra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 18:12:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.supra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 21:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc-mainnet.supra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:18:38 2026 GMT\n  hsts: null\ndomains:\n- domain: supra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/security/supra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Layer 1
- Oracles
- Web3
- Market Data
- Smart Contracts
- Verifiable Randomness
- Cross-Chain Bridge
- Automation
- Move
- Cryptocurrency
- DeFi
---
