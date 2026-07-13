---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: motional.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nuscenes.org
  spf: false
hosts:
- cert_expires: Aug 14 08:26:33 2026 GMT
  host: motional.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.nuscenes.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motional Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motional, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Motional
provider_slug: motional
slug: motional-domain-security
source_filename: motional-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motional.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 08:26:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: www.nuscenes.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: motional.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nuscenes.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motional/refs/heads/main/security/motional-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Vehicles
- Robotaxi
- Self-Driving
- Hyundai
- Aptiv
- Open Dataset
- nuScenes
- Lidar
---
