---
api_specs:
- filename: agentexchange-work-api-store-openapi.json
  format: json
  label: Agent Exchange API Store
  slug: api-store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/openapi/agentexchange-work-api-store-openapi.json
- filename: agentexchange-work-agent-planets-openapi.json
  format: json
  label: Agent Planets
  slug: agent-planets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/openapi/agentexchange-work-agent-planets-openapi.json
- filename: agentexchange-work-gatekeeper-oracle-openapi.json
  format: json
  label: Gatekeeper Oracle
  slug: gatekeeper-oracle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/openapi/agentexchange-work-gatekeeper-oracle-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentexchange.work
  spf: true
hosts:
- cert_expires: Dec 18 16:33:03 2026 GMT
  host: agentexchange.work
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 18:14:54 2026 GMT
  host: store.agentexchange.work
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 17:48:25 2026 GMT
  host: exchange.agentexchange.work
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agentexchange Work Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Exchange, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agent Exchange
provider_slug: agentexchange-work
slug: agentexchange-work-domain-security
source_filename: agentexchange-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentexchange.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:33:03 2026 GMT\n  hsts: false\n- host: store.agentexchange.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 18:14:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: exchange.agentexchange.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 17:48:25 2026 GMT\n  hsts: false\ndomains:\n- domain: agentexchange.work\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentexchange-work/refs/heads/main/security/agentexchange-work-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agentic Commerce
- x402
- MCP
- A2A
- AI Visibility
- Generative Engine Optimization
- Crypto
- Blockchain
- On-Chain Data
- Web Search
- Prediction Markets
- DeFi
- Macroeconomics
- Public Procurement
- Marketplace
- Agent-Native
---
