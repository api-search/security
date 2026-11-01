---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vialoop.in
  spf: true
hosts:
- cert_expires: Jan 15 00:11:42 2027 GMT
  host: vialoop.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vialoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ViaLoop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ViaLoop
provider_slug: vialoop
slug: vialoop-domain-security
source_filename: vialoop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vialoop.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 00:11:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vialoop.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/vialoop/security/vialoop-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Vehicle Tracking
- OBD Device
- Fuel Monitoring
- Driver Safety
- Car Sharing
- Multi‑vehicle
- GPS Tracking
---
