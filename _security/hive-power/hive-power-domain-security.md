---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hivepower.tech
  spf: true
hosts:
- cert_expires: Sep  4 21:24:57 2026 GMT
  host: hivepower.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hive Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hive Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hive Power
provider_slug: hive-power
slug: hive-power-domain-security
source_filename: hive-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hivepower.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 21:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hivepower.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hive-power/refs/heads/main/security/hive-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Virtual Power Plant
- Smart Charging
- Electric Vehicles
- Energy Flexibility
- Grid Services
- Battery Storage
- Demand Response
- IoT
---
