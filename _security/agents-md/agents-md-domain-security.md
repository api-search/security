---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agents.md
  spf: false
hosts:
- cert_expires: Sep  7 15:53:57 2026 GMT
  host: agents.md
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agents Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AGENTS.md, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AGENTS.md
provider_slug: agents-md
slug: agents-md-domain-security
source_filename: agents-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agents.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:53:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agents.md\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agents-md/refs/heads/main/security/agents-md-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Agents
- AI Copilot
- Coding Standards
- Developer Workflow
- Open Standard
- Documentation
---
