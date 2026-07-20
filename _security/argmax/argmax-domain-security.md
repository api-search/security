---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: argmaxinc.com
  spf: true
hosts:
- cert_expires: Aug 27 21:23:10 2026 GMT
  host: www.argmaxinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:08:43 2026 GMT
  host: app.argmaxinc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argmax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argmax, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Argmax
provider_slug: argmax
slug: argmax-domain-security
source_filename: argmax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.argmaxinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 21:23:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.argmaxinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:08:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: argmaxinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argmax/refs/heads/main/security/argmax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Artificial Intelligence
- Machine Learning
- On-Device Inference
- Speech Recognition
- Speech to Text
- Transcription
- Speaker Diarization
- Image Generation
- SDKs
- Apple Silicon
- Edge AI
---
