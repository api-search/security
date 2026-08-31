---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blynk.io
  spf: true
hosts:
- cert_expires: Sep 30 18:41:34 2026 GMT
  host: blynk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:48:02 2026 GMT
  host: docs.blynk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blynk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blynk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blynk
provider_slug: blynk
slug: blynk-domain-security
source_filename: blynk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blynk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:41:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.blynk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blynk.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blynk/refs/heads/main/security/blynk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Internet of Things
- No-Code
- Low-Code
- Connected Devices
- Device Management
- Fleet Management
- Mobile Apps
- Dashboards
- Telemetry
- Firmware
- Over The Air Updates
- White Label
- Embedded
- Smart Home
- Smart Buildings
- Smart Cities
- Industrial
- Agriculture
- Energy
---
