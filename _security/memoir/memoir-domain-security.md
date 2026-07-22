---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trymemoir.ai
  spf: false
hosts:
- cert_expires: Sep 14 11:38:22 2026 GMT
  host: www.trymemoir.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memoir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memoir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Memoir
provider_slug: memoir
slug: memoir-domain-security
source_filename: memoir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trymemoir.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trymemoir.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memoir/refs/heads/main/security/memoir-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketing
- Marketing Automation
- Artificial Intelligence
- Content Generation
- Developer Marketing
- SaaS
- Y Combinator
---
