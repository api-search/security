---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liv.tv
  spf: true
hosts:
- cert_expires: Sep 19 19:53:38 2026 GMT
  host: liv.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LIV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LIV
provider_slug: liv
slug: liv-domain-security
source_filename: liv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liv.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:53:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liv.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liv/refs/heads/main/security/liv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- XR
- Virtual Reality
- Mixed Reality
- Video Capture
- Live Streaming
- Game Engine SDK
- Unity
- Unreal Engine
- Meta Quest
---
