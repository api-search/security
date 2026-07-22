---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: source.dev
  spf: true
hosts:
- cert_expires: Oct 13 21:19:53 2026 GMT
  host: www.source.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcedev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Source.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Source.dev
provider_slug: sourcedev
slug: sourcedev-domain-security
source_filename: sourcedev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.source.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 21:19:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: source.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcedev/refs/heads/main/security/sourcedev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Build Systems
- Android
- AOSP
- DevOps
- Continuous Integration
- Embedded
- Automotive
- Artificial Intelligence
---
