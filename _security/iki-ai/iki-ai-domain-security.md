---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iki.ai
  spf: false
hosts:
- cert_expires: Sep  5 17:11:20 2026 GMT
  host: iki.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iki Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IKI AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: IKI AI
provider_slug: iki-ai
slug: iki-ai-domain-security
source_filename: iki-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iki.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:11:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iki.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iki-ai/refs/heads/main/security/iki-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Knowledge Management
- Research
- Productivity
- LLM
- Note Taking
- Team Collaboration
---
