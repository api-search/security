---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yaskawa-global.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yaskawa.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.yaskawa-global.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 13:16:36 2026 GMT
  host: www.yaskawa.com
  hsts: true
  hsts_max_age: 21600000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.motoman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yaskawa Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yaskawa / Motoman, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yaskawa / Motoman
provider_slug: yaskawa-robotics
slug: yaskawa-robotics-domain-security
source_filename: yaskawa-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yaskawa-global.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: www.yaskawa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:16:36 2026 GMT\n  hsts: true\n  hsts_max_age: 21600000\n- host: www.motoman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: yaskawa-global.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: yaskawa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yaskawa-robotics/refs/heads/main/security/yaskawa-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Industrial Robotics
- Industrial Automation
- Motion Control
- Servo Motors
- AC Drives
- Variable Frequency Drives
- Inverters
- Manufacturing
- Factory Automation
- SCARA
- Articulated Robots
- Delta Robots
- Collaborative Robots
- ROS 2
- micro-ROS
- MotoPlus
- Motoman
- Sigma-X
- Hardware
- SDK
---
