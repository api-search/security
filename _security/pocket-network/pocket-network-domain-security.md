---
api_specs:
- filename: pocket-network-path-gateway-api-openapi.yml
  format: yaml
  label: Pocket Network PATH Gateway API
  slug: pocket-network-path-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-path-gateway-api-openapi.yml
- filename: pocket-network-shannon-rpc-api-openapi.yml
  format: yaml
  label: Pocket Network Shannon RPC API
  slug: pocket-network-shannon-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-shannon-rpc-api-openapi.yml
- filename: pocket-network-cometbft-rpc-api-openapi.yml
  format: yaml
  label: Pocket Network CometBFT RPC API
  slug: pocket-network-cometbft-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-cometbft-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pocket.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grove.city
  spf: true
hosts:
- cert_expires: Aug 23 15:47:38 2026 GMT
  host: pocket.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:41:55 2026 GMT
  host: grove.city
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: path.grove.city
  https: false
kind: domain-security
layout: security
method: probed
name: Pocket Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pocket Network, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pocket Network
provider_slug: pocket-network
slug: pocket-network-domain-security
source_filename: pocket-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pocket.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:47:38 2026 GMT\n  hsts: false\n- host: grove.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:41:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: path.grove.city\n  https: false\ndomains:\n- domain: pocket.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: grove.city\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/security/pocket-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- RPC
- Decentralized Infrastructure
- Pocket Network
- Grove
- PATH
- Shannon
- Cosmos
- POKT
---
