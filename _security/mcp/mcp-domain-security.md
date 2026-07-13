---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: modelcontextprotocol.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smithery.ai
  spf: true
hosts:
- cert_expires: Sep  1 00:36:56 2026 GMT
  host: modelcontextprotocol.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 11:18:45 2026 GMT
  host: registry.modelcontextprotocol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 15:19:05 2026 GMT
  host: smithery.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Model Context Protocol (MCP), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Model Context Protocol (MCP)
provider_slug: mcp
slug: mcp-domain-security
source_filename: mcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:36:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: registry.modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:18:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modelcontextprotocol.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: smithery.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcp/refs/heads/main/security/mcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Model Context Protocol
- MCP
- AI Agents
- Tools
- Resources
- Prompts
- JSON-RPC
- Anthropic
- Standards
- Topic
---
