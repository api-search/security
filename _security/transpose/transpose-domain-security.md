---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Transpose Block API
  slug: transpose-block-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose Token API
  slug: transpose-token-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/verified-endpoints/token-api/overview/
- filename: openapi.yaml
  format: yaml
  label: Transpose NFT API
  slug: transpose-nft-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose ENS API
  slug: transpose-ens-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose Token Prices API
  slug: transpose-token-prices-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/verified-endpoints/token-prices-api/overview/
- filename: openapi.yaml
  format: yaml
  label: Transpose SQL Analytics API
  slug: transpose-sql-analytics-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: transpose.io
  spf: true
hosts:
- cert_expires: Aug 19 12:37:10 2026 GMT
  host: app.transpose.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 22:07:49 2026 GMT
  host: docs.transpose.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 02:00:22 2026 GMT
  host: api.transpose.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transpose Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transpose, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Transpose
provider_slug: transpose
slug: transpose-domain-security
source_filename: transpose-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.transpose.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 12:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.transpose.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:07:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.transpose.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 02:00:22 2026 GMT\n  hsts: null\ndomains:\n- domain: transpose.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transpose/refs/heads/main/security/transpose-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Blockchain
- NFT
- Cryptocurrency
- Web3
- Ethereum
- Token Transfers
- Smart Contracts
- Historical Data
- DeFi
- DEX
---
