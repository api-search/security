---
api_specs:
- filename: bscscan-accounts-api-openapi.yml
  format: yaml
  label: BscScan Accounts API
  slug: bscscan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-accounts-api-openapi.yml
- filename: bscscan-api-pro-endpoints-api-openapi.yml
  format: yaml
  label: BscScan API PRO Endpoints API
  slug: bscscan-api-pro-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-api-pro-endpoints-api-openapi.yml
- filename: bscscan-blocks-api-openapi.yml
  format: yaml
  label: BscScan Blocks API
  slug: bscscan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-blocks-api-openapi.yml
- filename: bscscan-contracts-api-openapi.yml
  format: yaml
  label: BscScan Contracts API
  slug: bscscan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-contracts-api-openapi.yml
- filename: bscscan-gas-tracker-api-openapi.yml
  format: yaml
  label: BscScan Gas Tracker API
  slug: bscscan-gas-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-gas-tracker-api-openapi.yml
- filename: bscscan-geth-parity-proxy-api-openapi.yml
  format: yaml
  label: BscScan Geth/Parity Proxy API
  slug: bscscan-geth-parity-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-geth-parity-proxy-api-openapi.yml
- filename: bscscan-logs-api-openapi.yml
  format: yaml
  label: BscScan Logs API
  slug: bscscan-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-logs-api-openapi.yml
- filename: bscscan-stats-api-openapi.yml
  format: yaml
  label: BscScan Stats API
  slug: bscscan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-stats-api-openapi.yml
- filename: bscscan-tokens-api-openapi.yml
  format: yaml
  label: BscScan Tokens API
  slug: bscscan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-tokens-api-openapi.yml
- filename: bscscan-transactions-api-openapi.yml
  format: yaml
  label: BscScan Transactions API
  slug: bscscan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: bscscan.com
  spf: true
hosts:
- cert_expires: Aug 20 18:17:02 2026 GMT
  host: bscscan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: api.bscscan.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 20 18:17:02 2026 GMT
  host: api-testnet.bscscan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bscscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BscScan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: BscScan
provider_slug: bscscan
slug: bscscan-domain-security
source_filename: bscscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bscscan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:17:02 2026 GMT\n  hsts: false\n- host: api.bscscan.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: false\n- host: api-testnet.bscscan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:17:02 2026 GMT\n  hsts: false\ndomains:\n- domain: bscscan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/security/bscscan-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- blockchain
- block-explorer
- BNB Smart Chain
- BSC
- BEP-20
- transactions
- smart-contracts
- DeFi
- EVM
---
