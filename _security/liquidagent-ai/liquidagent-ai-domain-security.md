---
api_specs:
- filename: liquidagent-ai-openapi.yml
  format: yaml
  label: Liquid Agent Tokenized Stock Index and Gas Sponsor API
  slug: liquid-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidagent-ai/refs/heads/main/openapi/liquidagent-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liquidagent.ai
  spf: true
hosts:
- cert_expires: Nov 17 04:19:49 2026 GMT
  host: liquidagent.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 05:11:00 2026 GMT
  host: api.liquidagent.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Liquidagent Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquid Agent, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liquid Agent
provider_slug: liquidagent-ai
slug: liquidagent-ai-domain-security
source_filename: liquidagent-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liquidagent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 04:19:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.liquidagent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 05:11:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liquidagent.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidagent-ai/refs/heads/main/security/liquidagent-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tokenized Stocks
- DeFi
- Investing
- Agentic Commerce
- x402
- Stablecoins
- Account Abstraction
- Gas Sponsorship
- Base
- Solana
- AI Agents
- Agent-Native
- A2A
- Portfolio Management
- Market Data
---
