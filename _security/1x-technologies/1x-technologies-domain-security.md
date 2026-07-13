---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 1x.tech
  spf: true
hosts:
- cert_expires: Sep 25 20:28:09 2026 GMT
  host: www.1x.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1X Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1X Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 1X Technologies
provider_slug: 1x-technologies
slug: 1x-technologies-domain-security
source_filename: 1x-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1x.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:28:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 1x.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1x-technologies/refs/heads/main/security/1x-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Robotics
- Humanoid Robots
- Consumer Robotics
- Home Robotics
- Embodied AI
- World Models
- NEO
- EVE
- ROS2
- Manufacturing
- Open Source
- 1xgpt
---
