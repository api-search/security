---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 4d-bios.com
  spf: true
  spf_record: v=spf1 include:spf.163.com -all
hosts:
- host: www.4d-bios.com
  hsts: true
  hsts_header: max-age=31536000
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  http_status: 200
  https: true
  server: nginx
- host: 4d-bios.com
  http_status: 200
  https: true
  server: nginx
- host: openapi.4d-bios.com
  http_status: 200
  https: true
  note: 4D Open Platform / 4D CUBE MS console (Ant Design Vue single-page app, login-gated)
- host: iot.4d-bios.com
  http_status: 200
  https: true
  note: IoT console (single-page app, login-gated)
- host: api.4d-bios.com
  http_status: null
  https: false
  note: DNS A record exists (120.55.48.120) but TCP connections to 80 and 443 time out from the probe point; no HTTP response was ever observed.
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: 4Dbios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4D Bios, probed live across 5 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 4D Bios
provider_slug: 4dbios
slug: 4dbios-domain-security
source_filename: 4dbios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the 4d-bios.com registrable domain and its console hosts\nnote: >-\n  The origin (Aliyun, Hangzhou) is intermittently unreachable from a US probe point — roughly one\n  request in three times out at the TCP layer. Every value below was re-probed until a real response\n  came back; an initial automated pass recorded https:false for www.4d-bios.com purely from those\n  timeouts and has been corrected here.\nhosts:\n- host: www.4d-bios.com\n  https: true\n  http_status: 200\n  server: nginx\n  hsts: true\n  hsts_header: max-age=31536000\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: 4d-bios.com\n  https: true\n  http_status: 200\n  server: nginx\n- host: openapi.4d-bios.com\n  https: true\n  http_status: 200\n  note: 4D Open Platform / 4D CUBE MS console (Ant Design Vue single-page app, login-gated)\n- host: iot.4d-bios.com\n  https: true\n  http_status: 200\n\
  \  note: IoT console (single-page app, login-gated)\n- host: api.4d-bios.com\n  https: false\n  http_status: null\n  note: >-\n    DNS A record exists (120.55.48.120) but TCP connections to 80 and 443 time out from the probe\n    point; no HTTP response was ever observed.\ndomains:\n- domain: 4d-bios.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.163.com -all\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4dbios/refs/heads/main/security/4dbios-domain-security.yml
summary_line: HSTS
tags:
- Company
- Agriculture
- Smart Agriculture
- Vertical Farming
- Plant Factory
- Controlled Environment Agriculture
- Internet of Things
- LED Lighting
- Hardware
- Manufacturing
---
