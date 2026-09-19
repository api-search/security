---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aidinrobotics.co.kr
  spf: true
hosts:
- cert_expires: Nov 23 04:00:50 2026 GMT
  host: www.aidinrobotics.co.kr
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aidinrobotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIDIN ROBOTICS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AIDIN ROBOTICS
provider_slug: aidinrobotics
slug: aidinrobotics-domain-security
source_filename: aidinrobotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aidinrobotics.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 04:00:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: aidinrobotics.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidinrobotics/refs/heads/main/security/aidinrobotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Sensors
- Hardware
- Industrial Automation
- Manufacturing
- Force and Torque Sensing
- Cobots
- Humanoid Robotics
- ROS
- SDK
- Company
---
