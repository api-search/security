---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Pocket Network Public RPC API
  slug: pocket-network-public-rpc-api
  spec_type: OpenAPI
  url: https://docs.pocket.network/developers/api-reference/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pocket.network
  spf: true
hosts:
- cert_expires: Aug 23 15:47:38 2026 GMT
  host: pocket.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:56:29 2026 GMT
  host: api.pocket.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 18:32:18 2026 GMT
  host: docs.pocket.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pokt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pocket Network, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pocket Network
provider_slug: pokt
slug: pokt-domain-security
source_filename: pokt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pocket.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:47:38 2026 GMT\n  hsts: false\n- host: api.pocket.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:56:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.pocket.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:32:18 2026 GMT\n  hsts: false\ndomains:\n- domain: pocket.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokt/refs/heads/main/security/pokt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- RPC
- Decentralized
- Web3
- Ethereum
- EVM
- Infrastructure
---
