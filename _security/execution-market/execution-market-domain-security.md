---
api_specs:
- filename: execution-market-openapi.yml
  format: yaml
  label: Execution Market REST API
  slug: execution-market-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/execution-market/refs/heads/main/openapi/execution-market-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: execution.market
  spf: false
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: execution.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.execution.market
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: docs.execution.market
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Execution Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ultravioleta DAO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ultravioleta DAO
provider_slug: execution-market
slug: execution-market-domain-security
source_filename: execution-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: execution.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.execution.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\n- host: docs.execution.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: execution.market\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/execution-market/refs/heads/main/security/execution-market-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI Agents
- Agent Marketplace
- Task Marketplace
- Gig Economy
- Payments
- Stablecoins
- Escrow
- x402
- MCP
- A2A
- Web3
- Blockchain
- DAO
- agent-native
---
