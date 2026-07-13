---
api_specs:
- filename: stellar-horizon-api.yml
  format: yaml
  label: Stellar Horizon API
  slug: horizon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/openapi/stellar-horizon-api.yml
- filename: stellar-anchor-platform-api.yml
  format: yaml
  label: Stellar Anchor Platform API
  slug: anchor-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/openapi/stellar-anchor-platform-api.yml
- filename: stellar-disbursement-platform-api.yml
  format: yaml
  label: Stellar Disbursement Platform API
  slug: disbursement-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/openapi/stellar-disbursement-platform-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stellar.org
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: developers.stellar.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: horizon.stellar.org
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: soroban-testnet.stellar.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stellar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stellar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stellar
provider_slug: stellar
slug: stellar-domain-security
source_filename: stellar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.stellar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: horizon.stellar.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\n- host: soroban-testnet.stellar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stellar.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/security/stellar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Cryptocurrency
- Decentralized Exchange
- Ledger
- Payments
- Smart Contracts
- Web3
---
