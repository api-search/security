---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imagineai.me
  spf: true
hosts:
- cert_expires: Sep 13 11:47:46 2026 GMT
  host: www.imagineai.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imagine Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imagine Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Imagine Ai
provider_slug: imagine-ai
slug: imagine-ai-domain-security
source_filename: imagine-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imagineai.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:47:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: imagineai.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imagine-ai/refs/heads/main/security/imagine-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Artificial Intelligence
- B2B
- Content Marketing
- LinkedIn
- Thought Leadership
- Social Media
- Lead Generation
- Persona
- Y Combinator
- SaaS
---
