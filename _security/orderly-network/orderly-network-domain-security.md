---
api_specs:
- filename: orderly-network-openapi-original.yml
  format: yaml
  label: Orderly EVM Trading API
  slug: orderly-evm-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderly-network/refs/heads/main/openapi/orderly-network-openapi-original.yml
- filename: orderly-network-strategy-vault-openapi-original.yml
  format: yaml
  label: Orderly Strategy Vault API
  slug: orderly-strategy-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderly-network/refs/heads/main/openapi/orderly-network-strategy-vault-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orderly.network
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: orderly.org
  spf: false
hosts:
- cert_expires: Sep  5 23:49:34 2026 GMT
  host: orderly.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:21:23 2026 GMT
  host: api.orderly.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 13:19:06 2026 GMT
  host: testnet-api.orderly.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orderly Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orderly Network, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orderly Network
provider_slug: orderly-network
slug: orderly-network-domain-security
source_filename: orderly-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orderly.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:49:34 2026 GMT\n  hsts: false\n- host: api.orderly.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:21:23 2026 GMT\n  hsts: false\n- host: testnet-api.orderly.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:19:06 2026 GMT\n  hsts: false\ndomains:\n- domain: orderly.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: orderly.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderly-network/refs/heads/main/security/orderly-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- DeFi
- Trading
- Perpetual Futures
- Derivatives
- Orderbook
- Web3
- Blockchain
- Liquidity
---
