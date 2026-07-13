---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: refact.ai
  spf: true
hosts:
- cert_expires: Sep 14 09:20:00 2026 GMT
  host: refact.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 09:19:58 2026 GMT
  host: docs.refact.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refact Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refact.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Refact.ai
provider_slug: refact-ai
slug: refact-ai-domain-security
source_filename: refact-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refact.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:20:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.refact.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:19:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: refact.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refact-ai/refs/heads/main/security/refact-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Coding Assistant
- AI Agent
- Autonomous Agents
- Code Completion
- Code Generation
- Developer Tools
- IDE
- VS Code
- JetBrains
- Self-Hosting
- On-Premise
- Open Source
- LSP
- MCP
- Model Context Protocol
- Fine-Tuning
- SWE-Bench
- RAG
---
