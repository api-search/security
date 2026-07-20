---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ai-coustics.com
  spf: true
hosts:
- cert_expires: Sep 18 18:53:56 2026 GMT
  host: ai-coustics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ai Coustics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ai-coustics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ai-coustics
provider_slug: ai-coustics
slug: ai-coustics-domain-security
source_filename: ai-coustics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-coustics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:53:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ai-coustics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-coustics/refs/heads/main/security/ai-coustics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai/Ml
- Audio
- Speech Enhancement
- Voice AI
- Speech Recognition
- SDK
- Real-Time
- Machine Learning
---
