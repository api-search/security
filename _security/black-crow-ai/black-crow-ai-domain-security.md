---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blackcrow.ai
  spf: true
hosts:
- cert_expires: Oct 11 19:25:10 2026 GMT
  host: www.blackcrow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Crow Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Crow AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Black Crow AI
provider_slug: black-crow-ai
slug: black-crow-ai-domain-security
source_filename: black-crow-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackcrow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackcrow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-crow-ai/refs/heads/main/security/black-crow-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Artificial Intelligence
- Machine Learning
- Marketing
- Advertising
- Personalization
- Conversion Optimization
---
