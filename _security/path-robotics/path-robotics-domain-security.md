---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: path-robotics.com
  spf: true
hosts:
- cert_expires: Sep 19 19:44:11 2026 GMT
  host: www.path-robotics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Path Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Path Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Path Robotics
provider_slug: path-robotics
slug: path-robotics-domain-security
source_filename: path-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.path-robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:44:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: path-robotics.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/path-robotics/refs/heads/main/security/path-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Welding
- Autonomous Welding
- Industrial Robotics
- Manufacturing
- Physical AI
- Embodied AI
- Reinforcement Learning
- World Models
- Obsidian
- Weld World Model
- Computer Vision
- LiDAR
- Defense
- Shipbuilding
- Energy Infrastructure
- Data Centers
- Heavy Industry
- Hardware
- Columbus Ohio
---
