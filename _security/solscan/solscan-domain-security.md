---
api_specs:
- filename: solscan-account-api-openapi.yml
  format: yaml
  label: Solscan Account API
  slug: solscan-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solscan/refs/heads/main/openapi/solscan-account-api-openapi.yml
- filename: solscan-block-api-openapi.yml
  format: yaml
  label: Solscan Block API
  slug: solscan-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solscan/refs/heads/main/openapi/solscan-block-api-openapi.yml
- filename: solscan-nft-api-openapi.yml
  format: yaml
  label: Solscan NFT API
  slug: solscan-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solscan/refs/heads/main/openapi/solscan-nft-api-openapi.yml
- filename: solscan-token-api-openapi.yml
  format: yaml
  label: Solscan Token API
  slug: solscan-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solscan/refs/heads/main/openapi/solscan-token-api-openapi.yml
- filename: solscan-transaction-api-openapi.yml
  format: yaml
  label: Solscan Transaction API
  slug: solscan-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solscan/refs/heads/main/openapi/solscan-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: solscan.io
  spf: true
hosts:
- cert_expires: Sep  9 01:57:11 2026 GMT
  host: solscan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 06:41:22 2026 GMT
  host: docs.solscan.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 01:57:11 2026 GMT
  host: public-api.solscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solscan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Solscan
provider_slug: solscan
slug: solscan-domain-security
source_filename: solscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 01:57:11 2026 GMT\n  hsts: null\n- host: docs.solscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.solscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 01:57:11 2026 GMT\n  hsts: false\ndomains:\n- domain: solscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solscan/refs/heads/main/security/solscan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Solana
- Explorer
- Onchain
- Tokens
- NFT
---
