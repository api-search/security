---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: manicule.dev
  spf: true
hosts:
- cert_expires: Sep 11 06:44:47 2026 GMT
  host: manicule.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manicule Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manicule, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Manicule
provider_slug: manicule
slug: manicule-domain-security
source_filename: manicule-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manicule.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: manicule.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manicule/refs/heads/main/security/manicule-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Relations
- Technical Documentation
- AI-Native Content
- DevTools
- Content Studio
- Y Combinator
---
