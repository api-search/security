---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abe.ai
  spf: true
hosts:
- cert_expires: Aug 27 23:18:18 2026 GMT
  host: abe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abe AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Abe AI
provider_slug: abe-ai
slug: abe-ai-domain-security
source_filename: abe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abe-ai/refs/heads/main/security/abe-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversational AI
- Financial Services
- Banking
- Chatbot
- Virtual Assistant
- Fintech
- Acquired
---
