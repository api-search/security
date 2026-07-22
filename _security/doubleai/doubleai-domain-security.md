---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doubleai.com
  spf: true
hosts:
- cert_expires: Sep 26 10:02:31 2026 GMT
  host: www.doubleai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Doubleai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doubleAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: doubleAI
provider_slug: doubleai
slug: doubleai-domain-security
source_filename: doubleai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doubleai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 10:02:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doubleai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubleai/refs/heads/main/security/doubleai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Machine Learning
- Deep Learning
- GPU Optimization
- Research
- Artificial Expert Intelligence
---
