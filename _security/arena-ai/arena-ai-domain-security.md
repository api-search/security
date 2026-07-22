---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arenaphysica.com
  spf: true
hosts:
- cert_expires: Aug 20 23:30:06 2026 GMT
  host: arenaphysica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arena Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arena AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arena AI
provider_slug: arena-ai
slug: arena-ai-domain-security
source_filename: arena-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arenaphysica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:30:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arenaphysica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arena-ai/refs/heads/main/security/arena-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Artificial Intelligence
- Hardware Engineering
- Radio Frequency
- Electromagnetics
- Model Context Protocol
- Applied Research
- Semiconductors
---
