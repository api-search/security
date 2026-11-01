---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clipwright.io
  spf: true
hosts:
- cert_expires: Jan  9 17:13:54 2027 GMT
  host: clipwright.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clipwright Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clipwright, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clipwright
provider_slug: clipwright
slug: clipwright-domain-security
source_filename: clipwright-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clipwright.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 17:13:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clipwright.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clipwright/security/clipwright-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Video
- UGC
- Automation
---
