---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: konos-sound.com
  spf: false
hosts:
- cert_expires: Sep 16 23:56:55 2026 GMT
  host: konos-sound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dotterel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotterel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dotterel
provider_slug: dotterel
slug: dotterel-domain-security
source_filename: dotterel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konos-sound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:56:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: konos-sound.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotterel/refs/heads/main/security/dotterel-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Audio
- Microphones
- Acoustics
- Hardware
- Drones
- Broadcast
- Film Production
---
