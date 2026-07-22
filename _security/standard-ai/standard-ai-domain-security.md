---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: standard.ai
  spf: true
hosts:
- cert_expires: Sep 19 23:36:30 2026 GMT
  host: standard.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Standard Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Standard AI
provider_slug: standard-ai
slug: standard-ai-domain-security
source_filename: standard-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standard.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:36:30 2026 GMT\n  hsts: false\ndomains:\n- domain: standard.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-ai/refs/heads/main/security/standard-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Computer Vision
- Artificial Intelligence
- Autonomous Checkout
- Retail Technology
---
