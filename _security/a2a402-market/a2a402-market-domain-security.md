---
api_specs:
- filename: a2a402-market-openapi.yml
  format: yaml
  label: A2A402 Production Agent Economy API
  slug: a2a402-production-agent-economy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2a402-market/refs/heads/main/openapi/a2a402-market-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: a2a402.market
  spf: false
hosts:
- cert_expires: Nov  7 00:17:17 2026 GMT
  host: a2a402.market
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: A2A402 Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A2A402, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: A2A402
provider_slug: a2a402-market
slug: a2a402-market-domain-security
source_filename: a2a402-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a2a402.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:17:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: a2a402.market\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a2a402-market/refs/heads/main/security/a2a402-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agent Marketplace
- A2A
- MCP
- Autonomous Agents
- Work Routing
- USDC
- Stablecoin Payments
- Blockchain
- Base
- Reputation
- Agent-Native
---
