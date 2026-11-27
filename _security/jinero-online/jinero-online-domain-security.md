---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jinero.online
  spf: true
hosts:
- cert_expires: Dec 23 01:04:21 2026 GMT
  host: jinero.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jinero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jinero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jinero
provider_slug: jinero-online
slug: jinero-online-domain-security
source_filename: jinero-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jinero.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 01:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jinero.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jinero-online/security/jinero-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design Tools
- Free
- Web
- Figma
- Image Processing
---
