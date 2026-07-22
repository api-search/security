---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uare.ai
  spf: true
hosts:
- cert_expires: Oct 10 17:14:20 2026 GMT
  host: uare.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uare Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uare.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Uare.ai
provider_slug: uare-ai
slug: uare-ai-domain-security
source_filename: uare-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uare.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:14:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: uare.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uare-ai/refs/heads/main/security/uare-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Personal AI
- Digital Twin
- Consumer
- Voice
- MCP
---
