---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: spartanradar.com
  spf: true
hosts:
- cert_expires: Nov 23 13:48:44 2026 GMT
  host: www.spartanradar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spartan Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spartan Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Spartan Radar
provider_slug: spartan-radar
slug: spartan-radar-domain-security
source_filename: spartan-radar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spartanradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 13:48:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spartanradar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spartan-radar/refs/heads/main/security/spartan-radar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Automotive
- Radar
- Sensors
- ADAS
- Autonomous Vehicles
- Perception
- Signal Processing
- Commercial Vehicles
- Embedded Software
- Safety
---
