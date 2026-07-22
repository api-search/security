---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: entropik.io
  spf: true
hosts:
- cert_expires: Oct 16 06:56:48 2026 GMT
  host: www.entropik.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entropik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entropik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Entropik
provider_slug: entropik
slug: entropik-domain-security
source_filename: entropik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entropik.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: entropik.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entropik/refs/heads/main/security/entropik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Emotion AI
- Consumer Insights
- User Research
- UX Research
- Market Research
- Insights Platform
- Eye Tracking
- SaaS
---
