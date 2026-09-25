---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adasky.com
  spf: true
hosts:
- cert_expires: Oct 28 16:19:49 2026 GMT
  host: www.adasky.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adasky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adasky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adasky
provider_slug: adasky
slug: adasky-domain-security
source_filename: adasky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adasky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:19:49 2026 GMT\n  hsts: false\ndomains:\n- domain: adasky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adasky/refs/heads/main/security/adasky-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Thermal Imaging
- Sensors
- ADAS
- Autonomous Vehicles
- Computer Vision
- Smart Cities
- Hardware
- Israel
- No Developer Program
---
