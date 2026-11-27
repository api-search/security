---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: codemouse.ai
  spf: false
hosts:
- cert_expires: Jan 23 07:53:07 2027 GMT
  host: codemouse.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CodeMouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeMouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CodeMouse
provider_slug: codemouse-ai
slug: codemouse-ai-domain-security
source_filename: codemouse-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codemouse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 07:53:07 2027 GMT\n  hsts: false\ndomains:\n- domain: codemouse.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/codemouse-ai/security/codemouse-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Code Review
- Artificial Intelligence
- GitHub
- Pull Requests
- Developer Tools
- LLM
---
