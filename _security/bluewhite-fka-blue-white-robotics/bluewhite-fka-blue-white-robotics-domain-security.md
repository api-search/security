---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bluewhite.ai
  spf: true
hosts:
- cert_expires: Oct  1 22:45:02 2026 GMT
  host: www.bluewhite.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluewhite Fka Blue White Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluewhite (fka Blue White Robotics), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bluewhite (fka Blue White Robotics)
provider_slug: bluewhite-fka-blue-white-robotics
slug: bluewhite-fka-blue-white-robotics-domain-security
source_filename: bluewhite-fka-blue-white-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluewhite.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:45:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bluewhite.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluewhite-fka-blue-white-robotics/refs/heads/main/security/bluewhite-fka-blue-white-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Autonomy
- Artificial Intelligence
- Agriculture
- AgTech
- Autonomous Vehicles
- Defense
- Unmanned Ground Vehicles
- Physical AI
---
