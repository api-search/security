---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lfaidata.foundation
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelcontextprotocol.io
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: lfaidata.foundation
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:36:56 2026 GMT
  host: modelcontextprotocol.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentic Ai Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentic AI Foundation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agentic AI Foundation
provider_slug: agentic-ai-foundation
slug: agentic-ai-foundation-domain-security
source_filename: agentic-ai-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lfaidata.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:36:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lfaidata.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: modelcontextprotocol.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/security/agentic-ai-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Linux Foundation
- Open Source
- Standards
- MCP
- Agentic AI
- Interoperability
---
