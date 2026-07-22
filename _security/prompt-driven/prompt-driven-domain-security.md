---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: promptdriven.ai
  spf: true
hosts:
- cert_expires: Sep 27 12:38:51 2026 GMT
  host: promptdriven.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prompt Driven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompt Driven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prompt Driven
provider_slug: prompt-driven
slug: prompt-driven-domain-security
source_filename: prompt-driven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptdriven.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:38:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: promptdriven.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prompt-driven/refs/heads/main/security/prompt-driven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Artificial Intelligence
- Code Generation
- Developer Experience
- CLI
- LLM
---
