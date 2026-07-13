---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verizonconnect.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fleetmatics.com
  spf: true
hosts:
- cert_expires: Aug 29 14:15:58 2026 GMT
  host: www.verizonconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:42:08 2026 GMT
  host: reveal-help.verizonconnect.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:48:32 2026 GMT
  host: fim.api.us.fleetmatics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verizon Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verizon Connect, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verizon Connect
provider_slug: verizon-connect
slug: verizon-connect-domain-security
source_filename: verizon-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verizonconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 14:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: reveal-help.verizonconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:42:08 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: fim.api.us.fleetmatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:48:32 2026 GMT\n  hsts: null\ndomains:\n- domain: verizonconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fleetmatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verizon-connect/refs/heads/main/security/verizon-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Telematics
- GPS Tracking
- Vehicle Tracking
- Fleet Tracking
- Verizon
- Fleetmatics
---
