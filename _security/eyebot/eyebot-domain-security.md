---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eyebot.co
  spf: false
hosts:
- cert_expires: Sep  7 14:54:14 2026 GMT
  host: www.eyebot.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eyebot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eyebot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Eyebot
provider_slug: eyebot
slug: eyebot-domain-security
source_filename: eyebot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eyebot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:54:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eyebot.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eyebot/refs/heads/main/security/eyebot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health Technology
- Vision Care
- Eye Care
- Medical Devices
- Kiosks
- Retail Technology
- Optometry
- Hardware
---
