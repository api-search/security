---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esphome.io
  spf: true
hosts:
- cert_expires: Dec  7 23:50:43 2026 GMT
  host: esphome.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Esphome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ESPHome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ESPHome
provider_slug: esphome
slug: esphome-domain-security
source_filename: esphome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esphome.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:50:43 2026 GMT\n  hsts: false\ndomains:\n- domain: esphome.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/esphome/security/esphome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Smart Home
- Home Automation
- Microcontrollers
- Open Source
- ESP32
- Home Assistant
---
