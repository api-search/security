---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clipember.com
  spf: true
hosts:
- cert_expires: Jan 18 14:20:51 2027 GMT
  host: clipember.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ClipEmber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClipEmber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ClipEmber
provider_slug: clipember-com
slug: clipember-com-domain-security
source_filename: clipember-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clipember.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 14:20:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clipember.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clipember-com/security/clipember-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Artificial Intelligence
- Video Editing
- Short-Form Video
- Captions
- Social Media
- MCP
---
