---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nanolumens.com
  spf: true
hosts:
- cert_expires: Oct  4 02:53:48 2026 GMT
  host: www.nanolumens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanolumens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NanoLumens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NanoLumens
provider_slug: nanolumens
slug: nanolumens-domain-security
source_filename: nanolumens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nanolumens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nanolumens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanolumens/refs/heads/main/security/nanolumens-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Signage
- LED Displays
- Display Manufacturing
- Audio Visual
- Digital Out Of Home
- Device Management
- Remote Monitoring
- Hardware
---
