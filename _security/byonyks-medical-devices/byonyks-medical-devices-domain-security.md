---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: byonyks.com
  spf: true
hosts:
- cert_expires: Nov 20 13:11:15 2026 GMT
  host: byonyks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Byonyks Medical Devices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byonyks Medical Devices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Byonyks Medical Devices
provider_slug: byonyks-medical-devices
slug: byonyks-medical-devices-domain-security
source_filename: byonyks-medical-devices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byonyks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 13:11:15 2026 GMT\n  hsts: false\ndomains:\n- domain: byonyks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byonyks-medical-devices/refs/heads/main/security/byonyks-medical-devices-domain-security.yml
summary_line: TLSv1.3
tags:
- Medical Devices
- Dialysis
- Healthcare
- Innovation
- FDA-cleared
---
