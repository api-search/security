---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: perseus.computer
  spf: false
hosts:
- cert_expires: Sep 18 14:36:24 2026 GMT
  host: perseus.computer
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perseus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perseus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Perseus
provider_slug: perseus
slug: perseus-domain-security
source_filename: perseus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perseus.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:36:24 2026 GMT\n  hsts: null\ndomains:\n- domain: perseus.computer\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perseus/refs/heads/main/security/perseus-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Developer Tools
- Code Search
- Semantic Search
- Coding Agents
- AI Agents
- Latent Space
- CLI
- Agent Skills
- Y Combinator
---
