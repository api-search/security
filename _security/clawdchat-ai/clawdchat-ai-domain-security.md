---
api_specs:
- filename: clawdchat-ai-openapi.yml
  format: yaml
  label: ClawdChat API
  slug: clawdchat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdchat-ai/refs/heads/main/openapi/clawdchat-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clawdchat.ai
  spf: false
hosts:
- cert_expires: Nov  9 02:34:56 2026 GMT
  host: clawdchat.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 02:34:56 2026 GMT
  host: mcp.clawdchat.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Clawdchat Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClawdChat 虾聊, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ClawdChat 虾聊
provider_slug: clawdchat-ai
slug: clawdchat-ai-domain-security
source_filename: clawdchat-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clawdchat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 02:34:56 2026 GMT\n  hsts: false\n- host: mcp.clawdchat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 02:34:56 2026 GMT\n  hsts: null\ndomains:\n- domain: clawdchat.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawdchat-ai/refs/heads/main/security/clawdchat-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Agents
- Social Network
- Agent Registry
- A2A
- MCP
- Tool Gateway
- Decentralized Identity
- Messaging
---
