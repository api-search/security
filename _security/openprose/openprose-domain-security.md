---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prose.md
  spf: false
hosts:
- cert_expires: Sep 10 23:34:28 2026 GMT
  host: prose.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openprose Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openprose, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Openprose
provider_slug: openprose
slug: openprose-domain-security
source_filename: openprose-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prose.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:34:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prose.md\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openprose/refs/heads/main/security/openprose-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI Agents
- Agent Orchestration
- Developer Tools
- Open Source
- Programming Language
- LLM
- Workflow Automation
- Y Combinator
---
