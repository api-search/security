---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: styleframe.ai
  spf: true
hosts:
- cert_expires: Oct  5 21:53:42 2026 GMT
  host: www.styleframe.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glyf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glyf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Glyf
provider_slug: glyf
slug: glyf-domain-security
source_filename: glyf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.styleframe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: styleframe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glyf/refs/heads/main/security/glyf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Creative Tools
- Motion Design
- Video Generation
- Generative AI
- Design
---
