---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: puzzlemed.com
  spf: true
hosts:
- cert_expires: Sep 16 11:30:59 2026 GMT
  host: www.puzzlemed.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puzzle Medical Devices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puzzle Medical Devices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Puzzle Medical Devices
provider_slug: puzzle-medical-devices
slug: puzzle-medical-devices-domain-security
source_filename: puzzle-medical-devices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.puzzlemed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:30:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: puzzlemed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle-medical-devices/refs/heads/main/security/puzzle-medical-devices-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Heart Failure
- Mechanical Circulatory Support
- Medical Technology
- Clinical Stage
- Canada
- Hardware
---
