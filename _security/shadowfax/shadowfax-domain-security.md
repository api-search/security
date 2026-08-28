---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shadowfax.ai
  spf: true
hosts:
- cert_expires: Nov 20 02:32:04 2026 GMT
  host: shadowfax.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shadowfax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shadowfax AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shadowfax AI
provider_slug: shadowfax
slug: shadowfax-domain-security
source_filename: shadowfax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shadowfax.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:32:04 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: shadowfax.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shadowfax/refs/heads/main/security/shadowfax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Business Intelligence
- Artificial Intelligence
- Data
- Agentic Analytics
- Data Engineering
- SaaS
---
