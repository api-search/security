---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kuka.com
  spf: true
hosts:
- cert_expires: Sep 16 11:14:02 2026 GMT
  host: www.kuka.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kuka Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KUKA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: KUKA
provider_slug: kuka-robotics
slug: kuka-robotics-domain-security
source_filename: kuka-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kuka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kuka.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuka-robotics/refs/heads/main/security/kuka-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Robotics
- Industrial Robots
- Industrial Automation
- Collaborative Robots
- Cobots
- Autonomous Mobile Robots
- Robot Controllers
- Robot Operating System
- KRL
- KSS
- KR C4
- KR C5
- iiQKA
- LBR iiwa
- PROFINET
- OPC UA
- Manufacturing
- Automotive
- Intralogistics
- Welding
- Palletizing
- Hardware
- Germany
- Midea
---
