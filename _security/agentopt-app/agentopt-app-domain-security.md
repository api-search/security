---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentopt.app
  spf: false
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: agentopt.app
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentopt App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Priorflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Priorflow
provider_slug: agentopt-app
slug: agentopt-app-domain-security
source_filename: agentopt-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentopt.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agentopt.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentopt-app/refs/heads/main/security/agentopt-app-domain-security.yml
summary_line: TLSv1.2
tags:
- AI Agents
- Agent Discovery
- Agent Selection
- A2A
- MCP
- Agent Orchestration
- Tool Ranking
- Semantic Search
- Agent-Native
---
