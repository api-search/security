---
api_specs:
- filename: anchor-x402-openapi.json
  format: json
  label: anchor-x402 API
  slug: anchor-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anchor-x402.com
  spf: true
hosts:
- cert_expires: Dec  4 01:26:27 2026 GMT
  host: anchor-x402.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.anchor-x402.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Anchor X402 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anchor-x402, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: anchor-x402
provider_slug: anchor-x402
slug: anchor-x402-domain-security
source_filename: anchor-x402-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchor-x402.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 01:26:27 2026 GMT\n  hsts: false\n- host: api.anchor-x402.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: anchor-x402.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/security/anchor-x402-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- x402
- Agents
- Payments
- Blockchain
- MCP
- Web3
- Pay Per Call
- Agent Payments
- Stablecoins
- Compliance
- Attestation
---
