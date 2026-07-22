---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sweep.dev
  spf: true
hosts:
- cert_expires: Oct  2 20:54:43 2026 GMT
  host: sweep.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sweep Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sweep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sweep
provider_slug: sweep-dev
slug: sweep-dev-domain-security
source_filename: sweep-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sweep.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:54:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sweep.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweep-dev/refs/heads/main/security/sweep-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Coding Assistant
- AI Developer Tools
- AI Agent
- Code Autocomplete
- Next Edit Suggestions
- JetBrains Plugin
- IntelliJ Platform
- VS Code Extension
- Zed Editor
- Code Review
- AI Commit Messages
- Inline Editing
- MCP
- Model Context Protocol
- Developer Productivity
- GitHub Issues
- Pull Request Automation
- Y Combinator
---
