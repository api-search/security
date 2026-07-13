---
api_specs:
- filename: ceramic.yaml
  format: yaml
  label: Ceramic HTTP API
  slug: ceramic-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ceramicnetwork/rust-ceramic/main/api/ceramic.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ceramic.network
  spf: true
hosts:
- cert_expires: Aug  2 20:13:56 2026 GMT
  host: ceramic.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 20:45:30 2026 GMT
  host: developers.ceramic.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceramic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ceramic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ceramic
provider_slug: ceramic
slug: ceramic-domain-security
source_filename: ceramic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceramic.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 20:13:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ceramic.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:45:30 2026 GMT\n  hsts: false\ndomains:\n- domain: ceramic.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/security/ceramic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Decentralized
- Web3
- Data Streams
- DID
- IPFS
- Blockchain
- Event Streaming
- ComposeDB
---
