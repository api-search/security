---
api_specs:
- filename: shapeshift-ethereum-openapi.json
  format: json
  label: ShapeShift Unchained — Ethereum (EVM) API
  slug: shapeshift-unchained-ethereum-evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-ethereum-openapi.json
- filename: shapeshift-bitcoin-openapi.json
  format: json
  label: ShapeShift Unchained — Bitcoin (UTXO) API
  slug: shapeshift-unchained-bitcoin-utxo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-bitcoin-openapi.json
- filename: shapeshift-solana-openapi.json
  format: json
  label: ShapeShift Unchained — Solana API
  slug: shapeshift-unchained-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-solana-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: shapeshift.com
  spf: true
hosts:
- cert_expires: Oct 14 17:34:04 2026 GMT
  host: shapeshift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 21:43:42 2026 GMT
  host: api.ethereum.shapeshift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 21:43:42 2026 GMT
  host: api.bitcoin.shapeshift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shapeshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shapeshift, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Shapeshift
provider_slug: shapeshift
slug: shapeshift-domain-security
source_filename: shapeshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shapeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:34:04 2026 GMT\n  hsts: false\n- host: api.ethereum.shapeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:43:42 2026 GMT\n  hsts: false\n- host: api.bitcoin.shapeshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:43:42 2026 GMT\n  hsts: false\ndomains:\n- domain: shapeshift.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/security/shapeshift-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Blockchain
- Bitcoin
- Ethereum
- Web3
- DeFi
- Wallet
- Trading
- Multichain
- API
---
