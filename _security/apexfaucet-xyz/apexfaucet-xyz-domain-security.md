---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apexfaucet.xyz
  spf: false
hosts:
- cert_expires: Dec 16 17:30:45 2026 GMT
  host: apexfaucet.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apexfaucet Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APEX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: APEX
provider_slug: apexfaucet-xyz
slug: apexfaucet-xyz-domain-security
source_filename: apexfaucet-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apexfaucet.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 17:30:45 2026 GMT\n  hsts: null\ndomains:\n- domain: apexfaucet.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apexfaucet-xyz/refs/heads/main/security/apexfaucet-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Blockchain
- Cryptocurrency
- Faucet
- Solana
- X1
- x402
- Micropayments
- Market Data
- Tokens
- AI Agents
- MCP
- A2A
---
