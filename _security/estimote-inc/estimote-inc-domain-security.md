---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: estimote.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: estimote.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: cloud.estimote.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Estimote Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estimote Inc, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Estimote Inc
provider_slug: estimote-inc
slug: estimote-inc-domain-security
source_filename: estimote-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estimote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: cloud.estimote.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: estimote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estimote-inc/refs/heads/main/security/estimote-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proximity
- Beacons
- Bluetooth
- BLE
- UWB
- Ultra Wideband
- LTE
- IoT
- Indoor Location
- Asset Tracking
- RTLS
- Sensors
- Hardware
---
