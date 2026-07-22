---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wabi.ai
  spf: true
hosts:
- cert_expires: Sep 13 22:19:53 2026 GMT
  host: wabi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wabi
provider_slug: wabi
slug: wabi-domain-security
source_filename: wabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wabi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:19:53 2026 GMT\n  hsts: false\ndomains:\n- domain: wabi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wabi/refs/heads/main/security/wabi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- App Builder
- No-Code
- Personal Software
- Mini Apps
- Consumer
- Generative AI
---
