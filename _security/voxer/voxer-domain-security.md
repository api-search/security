---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: voxer.com
  spf: true
hosts:
- cert_expires: Nov 16 02:00:14 2026 GMT
  host: www.voxer.com
  hsts: true
  hsts_max_age: 900
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voxer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voxer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Voxer
provider_slug: voxer
slug: voxer-domain-security
source_filename: voxer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voxer.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 02:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 900\ndomains:\n- domain: voxer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxer/refs/heads/main/security/voxer-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Communications
- Push-To-Talk
- Walkie-Talkie
- Voice
- Messaging
- Mobile
- SDK
---
