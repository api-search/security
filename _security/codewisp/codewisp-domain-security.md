---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codewisp.ai
  spf: true
hosts:
- cert_expires: Sep  8 12:15:17 2026 GMT
  host: codewisp.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codewisp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codewisp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Codewisp
provider_slug: codewisp
slug: codewisp-domain-security
source_filename: codewisp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codewisp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:15:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: codewisp.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codewisp/refs/heads/main/security/codewisp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Game Development
- Artificial Intelligence
- Generative AI
- No-Code
- Games
- Developer Tools
- Y Combinator
---
