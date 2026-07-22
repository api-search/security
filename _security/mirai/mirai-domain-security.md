---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trymirai.com
  spf: false
hosts:
- cert_expires: Sep 27 13:00:45 2026 GMT
  host: trymirai.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 12 05:07:08 2026 GMT
  host: docs.trymirai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mirai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mirai
provider_slug: mirai
slug: mirai-domain-security
source_filename: mirai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trymirai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 13:00:45 2026 GMT\n  hsts: false\n- host: docs.trymirai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 05:07:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trymirai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirai/refs/heads/main/security/mirai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- On-Device AI
- Inference
- LLM
- SDK
- Machine Learning
- Edge AI
- Apple Silicon
- Text to Speech
---
