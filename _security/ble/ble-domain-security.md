---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bluetooth.com
  spf: true
hosts:
- cert_expires: Aug 30 06:23:29 2026 GMT
  host: www.bluetooth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BLE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BLE
provider_slug: ble
slug: ble-domain-security
source_filename: ble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluetooth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:23:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bluetooth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ble/refs/heads/main/security/ble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- BLE
- Bluetooth
- Embedded
- IoT
- Protocols
- Standards
- Wireless
---
