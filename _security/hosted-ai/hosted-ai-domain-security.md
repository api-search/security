---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hosted.ai
  spf: true
hosts:
- cert_expires: Sep 27 10:47:34 2026 GMT
  host: hosted.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hosted Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hosted·ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hosted·ai
provider_slug: hosted-ai
slug: hosted-ai-domain-security
source_filename: hosted-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hosted.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hosted.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hosted-ai/refs/heads/main/security/hosted-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- GPU
- GPUaaS
- Cloud Infrastructure
- Neocloud
- Machine Learning
- AI Infrastructure
- Multi-Tenancy
- Service Providers
---
