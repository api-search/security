---
api_specs:
- filename: sponge-openapi-original.json
  format: json
  label: Sponge Wallet API
  slug: sponge-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sponge/refs/heads/main/openapi/sponge-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: paysponge.com
  spf: true
hosts:
- cert_expires: Oct  8 07:19:10 2026 GMT
  host: api.wallet.paysponge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sponge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sponge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sponge
provider_slug: sponge
slug: sponge-domain-security
source_filename: sponge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.wallet.paysponge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:19:10 2026 GMT\n  hsts: null\ndomains:\n- domain: paysponge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sponge/refs/heads/main/security/sponge-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agent Payments
- AI Agents
- Wallets
- Cryptocurrency
- Payments
- Stablecoins
- x402
- MPP
- Financial Infrastructure
- MCP
- Fintech
- Cards
- Onramp
---
