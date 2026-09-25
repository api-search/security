---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: velvt.ai
  spf: true
hosts:
- cert_expires: Nov 17 14:39:02 2026 GMT
  host: velvt.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Velvt Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velvt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Velvt
provider_slug: velvt-ai
slug: velvt-ai-domain-security
source_filename: velvt-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velvt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 14:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: velvt.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velvt-ai/refs/heads/main/security/velvt-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Agents
- Agent Networks
- Agent Evaluation
- MCP
- A2A
- Behavioral Evidence
- Agent Assurance
- Multi-Agent Collaboration
- Observability
- Reputation
---
