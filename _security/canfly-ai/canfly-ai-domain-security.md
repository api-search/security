---
api_specs:
- filename: canfly-ai-openapi.yml
  format: yaml
  label: CanFly.ai Agent Skill Marketplace API
  slug: canfly-agent-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canfly-ai/refs/heads/main/openapi/canfly-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: canfly.ai
  spf: true
hosts:
- cert_expires: Nov 29 07:53:37 2026 GMT
  host: canfly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canfly Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CanFly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CanFly
provider_slug: canfly-ai
slug: canfly-ai-domain-security
source_filename: canfly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canfly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 07:53:37 2026 GMT\n  hsts: false\ndomains:\n- domain: canfly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canfly-ai/refs/heads/main/security/canfly-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Agents
- AI Agents
- Agentic Commerce
- Marketplace
- A2A
- MCP
- USDC
- OpenClaw
- Agent-Native
- Taiwan
---
