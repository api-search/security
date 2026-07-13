---
api_specs:
- filename: art-blocks-token-api.json
  format: json
  label: Art Blocks Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/art-blocks/refs/heads/main/openapi/art-blocks-token-api.json
- filename: art-blocks-generator-api.json
  format: json
  label: Art Blocks Generator API
  slug: generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/art-blocks/refs/heads/main/openapi/art-blocks-generator-api.json
- filename: art-blocks-media-proxy-api.json
  format: json
  label: Art Blocks Media Proxy API
  slug: media-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/art-blocks/refs/heads/main/openapi/art-blocks-media-proxy-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: artblocks.io
  spf: true
hosts:
- cert_expires: Sep 18 16:59:35 2026 GMT
  host: www.artblocks.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:33:48 2026 GMT
  host: docs.artblocks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 22:57:07 2026 GMT
  host: token.artblocks.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Art Blocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Art Blocks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Art Blocks
provider_slug: art-blocks
slug: art-blocks-domain-security
source_filename: art-blocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artblocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.artblocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: token.artblocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:57:07 2026 GMT\n  hsts: null\ndomains:\n- domain: artblocks.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/art-blocks/refs/heads/main/security/art-blocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Generative Art
- NFT
- On-Chain Art
- Blockchain
- Ethereum
- Arbitrum
- Base
- GraphQL
- Token Metadata
- Web3
- Smart Contracts
- The Graph
- MCP
---
