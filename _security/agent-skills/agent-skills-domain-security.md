---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claude.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthropic.com
  spf: true
hosts:
- cert_expires: Sep 24 00:48:33 2026 GMT
  host: platform.claude.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:45:51 2026 GMT
  host: api.anthropic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 02:51:21 2026 GMT
  host: adk.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agent Skills Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Skills, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Agent Skills
provider_slug: agent-skills
slug: agent-skills-domain-security
source_filename: agent-skills-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.claude.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:48:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:45:51 2026 GMT\n  hsts: null\n- host: adk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 02:51:21 2026 GMT\n  hsts: false\ndomains:\n- domain: claude.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: anthropic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-skills/refs/heads/main/security/agent-skills-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Skills
- AI Agents
- Tool Use
- Function Calling
- MCP
- Agentic AI
- Automation
---
