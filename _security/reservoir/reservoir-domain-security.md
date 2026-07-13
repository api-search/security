---
api_specs:
- filename: llms.txt
  format: yaml
  label: Reservoir NFT API
  slug: reservoir-nft-api
  spec_type: OpenAPI
  url: https://reservoirprotocol.readme.io/llms.txt
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reservoir.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reservoir.tools
  spf: true
hosts:
- host: reservoir.dev
  https: false
- host: api.reservoir.tools
  https: false
kind: domain-security
layout: security
method: probed
name: Reservoir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reservoir, probed live across 2 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Reservoir
provider_slug: reservoir
slug: reservoir-domain-security
source_filename: reservoir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reservoir.dev\n  https: false\n- host: api.reservoir.tools\n  https: false\ndomains:\n- domain: reservoir.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: reservoir.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/security/reservoir-domain-security.yml
summary_line: DMARC
tags:
- NFT
- Blockchain
- Marketplace
- Ethereum
- EVM
- Liquidity
- Order Book
- Web3
- DeFi
- Trading
- Data API
---
