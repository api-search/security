---
api_specs:
- filename: manifold-oauth2-authentication-api.yml
  format: yaml
  label: Manifold OAuth2 Authentication API
  slug: oauth2-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manifold/refs/heads/main/openapi/manifold-oauth2-authentication-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: manifold.xyz
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: manifoldxyz.dev
  spf: false
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: manifold.xyz
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  2 05:26:04 2026 GMT
  host: docs.manifold.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: apps.api.manifoldxyz.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Manifold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manifold, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Manifold
provider_slug: manifold
slug: manifold-domain-security
source_filename: manifold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manifold.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: docs.manifold.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:26:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apps.api.manifoldxyz.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: manifold.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: manifoldxyz.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manifold/refs/heads/main/security/manifold-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- NFT
- Creator Tools
- Smart Contracts
- Blockchain
- Web3
- Ethereum
- ERC721
- ERC1155
- Royalties
- Marketplace
- Minting
- OpenSea
- Base
- Optimism
---
