---
api_specs:
- filename: agentic-ai-foundation-mcp-registry-openapi.yaml
  format: yaml
  label: Official MCP Registry API
  slug: mcp-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/openapi/agentic-ai-foundation-mcp-registry-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aaif.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelcontextprotocol.io
  spf: true
hosts:
- cert_expires: Oct 18 15:58:23 2026 GMT
  host: aaif.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 16:36:50 2026 GMT
  host: modelcontextprotocol.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 10:20:44 2026 GMT
  host: registry.modelcontextprotocol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentic Ai Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentic AI Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Agentic AI Foundation
provider_slug: agentic-ai-foundation
slug: agentic-ai-foundation-domain-security
source_filename: agentic-ai-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaif.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:58:23 2026 GMT\n  hsts: false\n- host: modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 16:36:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: registry.modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 10:20:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aaif.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: modelcontextprotocol.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/security/agentic-ai-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Linux Foundation
- Open-Source
- Standards
- MCP
- Agentic AI
- Interoperability
- Agent Protocols
- A2A
- AGENTS.md
- Open Governance
---
