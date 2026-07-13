---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: global.abb
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abb.com
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: global.abb
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: new.abb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: developercenter.robotstudio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abb Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABB Robotics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ABB Robotics
provider_slug: abb-robotics
slug: abb-robotics-domain-security
source_filename: abb-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: global.abb\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: new.abb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developercenter.robotstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: global.abb\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: abb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abb-robotics/refs/heads/main/security/abb-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Industrial Robotics
- Industrial Automation
- Manufacturing
- Robot Controllers
- OmniCore
- RobotStudio
- RAPID
- Collaborative Robots
- Cobots
- Welding
- Painting
- Material Handling
- Picking and Packing
- Discrete Automation
- Robot Web Services
- REST
- WebSockets
---
