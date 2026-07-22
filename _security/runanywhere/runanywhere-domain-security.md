---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: runanywhere.ai
  spf: false
hosts:
- cert_expires: Aug 27 09:24:00 2026 GMT
  host: www.runanywhere.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 03:51:57 2026 GMT
  host: docs.runanywhere.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- host: api.runanywhere.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Runanywhere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RunAnywhere, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RunAnywhere
provider_slug: runanywhere
slug: runanywhere-domain-security
source_filename: runanywhere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.runanywhere.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 27 09:24:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.runanywhere.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 03:51:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.runanywhere.ai\n  https: false\ndomains:\n- domain: runanywhere.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runanywhere/refs/heads/main/security/runanywhere-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- On-Device AI
- Inference
- Machine Learning
- SDK
- Mobile
- Edge AI
- LLM
- Speech
- Y Combinator
---
