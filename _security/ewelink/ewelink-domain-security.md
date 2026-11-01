---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ewelink.cc
  spf: true
hosts:
- cert_expires: Jan 13 15:34:04 2027 GMT
  host: ewelink.cc
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ewelink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eWeLink (ITEAD / Sonoff), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: eWeLink (ITEAD / Sonoff)
provider_slug: ewelink
slug: ewelink-domain-security
source_filename: ewelink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ewelink.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:34:04 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ewelink.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ewelink/security/ewelink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Home
- IoT
- Cloud Platform
- Automation
- Voice Assistant Integration
- Company
---
