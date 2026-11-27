---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: filtrix.ai
  spf: true
hosts:
- cert_expires: Dec 31 06:15:13 2026 GMT
  host: filtrix.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Filtrix AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filtrix AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Filtrix AI
provider_slug: filtrix-ai
slug: filtrix-ai-domain-security
source_filename: filtrix-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filtrix.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: filtrix.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/filtrix-ai/security/filtrix-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Creative Tools
- Marketing
- Advertising
- Image Editing
- MCP
- Generative AI
---
