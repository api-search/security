---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simberobotics.com
  spf: true
hosts:
- cert_expires: Oct 19 17:37:59 2026 GMT
  host: www.simberobotics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simbe Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simbe Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Simbe Robotics
provider_slug: simbe-robotics
slug: simbe-robotics-domain-security
source_filename: simbe-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simberobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 17:37:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: simberobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simbe-robotics/refs/heads/main/security/simbe-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Retail
- Inventory
- Computer Vision
- Artificial Intelligence
- Store Intelligence
- RFID
- Supply Chain
- Physical AI
---
