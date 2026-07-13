---
api_specs:
- filename: ethereum-json-rpc-openapi.yml
  format: yaml
  label: Ethereum JSON-RPC API
  slug: ethereum-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethereum/refs/heads/main/openapi/ethereum-json-rpc-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ethereum.org
  spf: true
hosts:
- cert_expires: Sep 30 07:48:51 2026 GMT
  host: ethereum.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ethereum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethereum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ethereum
provider_slug: ethereum
slug: ethereum-domain-security
source_filename: ethereum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethereum.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:48:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ethereum.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethereum/refs/heads/main/security/ethereum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- DeFi
- Ethereum
- JSON-RPC
- Smart Contracts
- Web3
---
