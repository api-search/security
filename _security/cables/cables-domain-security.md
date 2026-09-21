---
api_specs:
- filename: cables-openapi.yml
  format: yaml
  label: TensorFlow.js Social Media MCP Server
  slug: tensorflowjs-social-media-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cables/refs/heads/main/openapi/cables-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cables.live
  spf: true
hosts:
- cert_expires: Dec  7 06:51:51 2026 GMT
  host: mcp.cables.live
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cables Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cables, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cables
provider_slug: cables
slug: cables-domain-security
source_filename: cables-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp.cables.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 06:51:51 2026 GMT\n  hsts: null\ndomains:\n- domain: cables.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cables/refs/heads/main/security/cables-domain-security.yml
summary_line: TLSv1.3
tags:
- MCP Server
- agent-native
- x402
- pay-per-call
- Machine-Learning
- tensorflow-js
- NLP
- Computer-Vision
- Social Media Analytics
- OpenAPI
- Solana
- Crypto Payments
- testnet-devnet
---
