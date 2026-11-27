---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: decibelshield.app
  spf: false
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: decibelshield.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Decibel Shield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decibel Shield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Decibel Shield
provider_slug: decibelshield-app
slug: decibelshield-app-domain-security
source_filename: decibelshield-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decibelshield.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: decibelshield.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/decibelshield-app/security/decibelshield-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sound Meter
- Occupational Safety
- Health
- Web App
- Audio Measurement
---
