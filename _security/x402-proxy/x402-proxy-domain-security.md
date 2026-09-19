---
api_specs:
- filename: x402-proxy-openapi-original.json
  format: json
  label: x402-proxy API
  slug: x402-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x402-proxy/refs/heads/main/openapi/x402-proxy-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgemesh.io
  spf: true
hosts:
- cert_expires: Dec  8 18:18:26 2026 GMT
  host: proxy.forgemesh.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: X402 Proxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for x402-proxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: x402-proxy
provider_slug: x402-proxy
slug: x402-proxy-domain-security
source_filename: x402-proxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proxy.forgemesh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 18:18:26 2026 GMT\n  hsts: false\ndomains:\n- domain: forgemesh.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-proxy/refs/heads/main/security/x402-proxy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- api-monetization
- payments
- x402
- micropayments
- usdc
- stablecoin
- base-l2
- blockchain
- web3
- agentic-commerce
- ai-agents
- api-proxy
- api-gateway
- pay-per-use
---
