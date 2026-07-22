---
api_specs:
- filename: setup
  format: yaml
  label: Quai Network JSON-RPC API
  slug: quai-network-json-rpc-api
  spec_type: Postman
  url: https://docs.qu.ai/build/apis/postman/setup
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qu.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quai.network
  spf: true
hosts:
- cert_expires: Oct 15 15:26:17 2026 GMT
  host: qu.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 00:31:54 2026 GMT
  host: docs.qu.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: rpc.quai.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quai Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quai Network, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quai Network
provider_slug: quai-network
slug: quai-network-domain-security
source_filename: quai-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.quai.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: qu.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: quai.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quai-network/refs/heads/main/security/quai-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Layer 1
- Blockchain
- Cryptocurrency
- Web3
- Smart Contracts
- EVM
- JSON-RPC
- Proof of Work
- Developer Tools
---
