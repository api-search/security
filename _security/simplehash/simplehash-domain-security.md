---
api_specs:
- filename: overview
  format: yaml
  label: SimpleHash NFT & Token API
  slug: nft-api
  spec_type: OpenAPI
  url: https://docs.simplehash.com/reference/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplehash.com
  spf: true
hosts:
- cert_expires: Aug 19 22:13:52 2026 GMT
  host: simplehash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:25:36 2026 GMT
  host: api.simplehash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplehash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleHash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SimpleHash
provider_slug: simplehash
slug: simplehash-domain-security
source_filename: simplehash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simplehash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 22:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.simplehash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:25:36 2026 GMT\n  hsts: null\ndomains:\n- domain: simplehash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplehash/refs/heads/main/security/simplehash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- NFT
- Blockchain
- Web3
- Cryptocurrency
- Token
- Metadata
- Multi-chain
- Ethereum
- Solana
- Base
- Polygon
---
