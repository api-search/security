---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: obot.ai
  spf: true
hosts:
- cert_expires: Sep  1 07:11:38 2026 GMT
  host: obot.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 02:35:32 2026 GMT
  host: docs.obot.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Obot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Obot
provider_slug: obot
slug: obot-domain-security
source_filename: obot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:11:38 2026 GMT\n  hsts: false\n- host: docs.obot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:35:32 2026 GMT\n  hsts: false\ndomains:\n- domain: obot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obot/refs/heads/main/security/obot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- MCP Gateway
- Open Source
- Agent Governance
- Access Control
- Developer Tools
---
