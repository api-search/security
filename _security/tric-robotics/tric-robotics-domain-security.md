---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tricrobotics.com
  spf: true
hosts:
- cert_expires: Apr  1 15:02:32 2027 GMT
  host: www.tricrobotics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tric Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TRIC Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TRIC Robotics
provider_slug: tric-robotics
slug: tric-robotics-domain-security
source_filename: tric-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tricrobotics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  1 15:02:32 2027 GMT\n  hsts: false\ndomains:\n- domain: tricrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tric-robotics/refs/heads/main/security/tric-robotics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Robotics
- Agriculture
- AgTech
- Automation
- Autonomous Vehicles
- Pest Control
- Sustainability
- Robotics as a Service
---
