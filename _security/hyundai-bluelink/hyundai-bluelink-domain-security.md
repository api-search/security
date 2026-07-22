---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hyundaiusa.com
  spf: true
hosts:
- cert_expires: Aug 22 07:11:19 2026 GMT
  host: owners.hyundaiusa.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyundai Bluelink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyundai Bluelink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hyundai Bluelink
provider_slug: hyundai-bluelink
slug: hyundai-bluelink-domain-security
source_filename: hyundai-bluelink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owners.hyundaiusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:11:19 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: hyundaiusa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyundai-bluelink/refs/heads/main/security/hyundai-bluelink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Vehicles
- Telematics
- Automotive
- Remote Vehicle Control
- Vehicle Diagnostics
- Electric Vehicles
- EV Charging
- Stolen Vehicle Recovery
- Automatic Collision Notification
- Roadside Assistance
- In-Vehicle Wi-Fi
- Navigation
- Smart Home Integration
- Voice Assistant
- Hyundai
- Bluelink
---
