---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trueface.ai
  spf: true
hosts:
- cert_expires: Sep 13 04:27:43 2026 GMT
  host: trueface.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chui Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chui, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chui
provider_slug: chui
slug: chui-domain-security
source_filename: chui-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trueface.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:27:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trueface.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chui/refs/heads/main/security/chui-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Facial Recognition
- Computer Vision
- Machine Learning
- Identity Verification
- Biometrics
- SDK
- Security
---
