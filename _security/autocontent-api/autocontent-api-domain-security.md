---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autocontentapi.com
  spf: true
hosts:
- cert_expires: Sep  4 21:03:49 2026 GMT
  host: autocontentapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 02:53:58 2026 GMT
  host: api.autocontentapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autocontent Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoContent API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AutoContent API
provider_slug: autocontent-api
slug: autocontent-api-domain-security
source_filename: autocontent-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autocontentapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 21:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.autocontentapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:53:58 2026 GMT\n  hsts: false\ndomains:\n- domain: autocontentapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/security/autocontent-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Audio
- Content Generation
- Podcasts
- Video
- Generative AI
- Text to Speech
- Automation
---
