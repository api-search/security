---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getsafari.ai
  spf: true
hosts:
- cert_expires: Sep  5 20:01:26 2026 GMT
  host: www.getsafari.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safari Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safari Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Safari Ai
provider_slug: safari-ai
slug: safari-ai-domain-security
source_filename: safari-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getsafari.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:01:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getsafari.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safari-ai/refs/heads/main/security/safari-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computer Vision
- Video Analytics
- Physical Operations
- Retail Analytics
- People Counting
- Operational Intelligence
- Vision AI
---
