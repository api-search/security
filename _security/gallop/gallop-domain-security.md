---
api_specs:
- filename: gallop-ethereum-api-openapi.yml
  format: yaml
  label: Gallop Ethereum API
  slug: gallop-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-ethereum-api-openapi.yml
- filename: gallop-polygon-api-openapi.yml
  format: yaml
  label: Gallop Polygon API
  slug: gallop-polygon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-polygon-api-openapi.yml
- filename: gallop-solana-api-openapi.yml
  format: yaml
  label: Gallop Solana API
  slug: gallop-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-solana-api-openapi.yml
- filename: gallop-starknet-api-openapi.yml
  format: yaml
  label: Gallop Starknet API
  slug: gallop-starknet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-starknet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: higallop.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gallop.run
  spf: true
hosts:
- host: higallop.com
  https: false
- host: api.prod.gallop.run
  https: false
kind: domain-security
layout: security
method: probed
name: Gallop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gallop, probed live across 2 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gallop
provider_slug: gallop
slug: gallop-domain-security
source_filename: gallop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: higallop.com\n  https: false\n- host: api.prod.gallop.run\n  https: false\ndomains:\n- domain: higallop.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: gallop.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/security/gallop-domain-security.yml
summary_line: DMARC
tags:
- Company
- Developer Tools
- NFT
- Blockchain
- Web3
- Data
- Analytics
- Crypto
- Ethereum
- Solana
---
