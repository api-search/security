---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bith.ai
  spf: false
hosts:
- cert_expires: Oct 14 16:11:29 2026 GMT
  host: bith.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bithtv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bith.tv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: bith.tv
provider_slug: bithtv
slug: bithtv-domain-security
source_filename: bithtv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bith.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:11:29 2026 GMT\n  hsts: false\ndomains:\n- domain: bith.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bithtv/refs/heads/main/security/bithtv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Video Editing
- Content Creation
- AI
- Media
- Social Media
- Creator Tools
---
