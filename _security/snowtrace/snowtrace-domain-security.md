---
api_specs:
- filename: snowtrace-accounts-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Accounts API
  slug: snowtrace-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-accounts-api-openapi.yml
- filename: snowtrace-blocks-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Blocks API
  slug: snowtrace-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-blocks-api-openapi.yml
- filename: snowtrace-contracts-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Contracts API
  slug: snowtrace-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-contracts-api-openapi.yml
- filename: snowtrace-logs-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Logs API
  slug: snowtrace-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-logs-api-openapi.yml
- filename: snowtrace-proxy-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Proxy API
  slug: snowtrace-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-proxy-api-openapi.yml
- filename: snowtrace-stats-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Stats API
  slug: snowtrace-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-stats-api-openapi.yml
- filename: snowtrace-tokens-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Tokens API
  slug: snowtrace-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-tokens-api-openapi.yml
- filename: snowtrace-transactions-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Transactions API
  slug: snowtrace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: snowtrace.io
  spf: false
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: snowtrace.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snowtrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Routescan (Snowtrace), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Routescan (Snowtrace)
provider_slug: snowtrace
slug: snowtrace-domain-security
source_filename: snowtrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snowtrace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snowtrace.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/security/snowtrace-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Blockchain
- Explorer
- Avalanche
- EVM
- Multichain
- Web3
- Transaction
- Smart Contracts
- NFTs
- DeFi
---
