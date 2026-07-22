---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: standardbots.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: robot-control-box.local
  spf: false
hosts:
- cert_expires: Oct 14 17:39:48 2026 GMT
  host: standardbots.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 06:14:21 2026 GMT
  host: docs.standardbots.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: robot-control-box.local
  https: false
kind: domain-security
layout: security
method: probed
name: Standard Bots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Bots, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Standard Bots
provider_slug: standard-bots
slug: standard-bots-domain-security
source_filename: standard-bots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standardbots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:39:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.standardbots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:14:21 2026 GMT\n  hsts: false\n- host: robot-control-box.local\n  https: false\ndomains:\n- domain: standardbots.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: robot-control-box.local\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-bots/refs/heads/main/security/standard-bots-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Industrial Automation
- Robotic Arm
- Manufacturing
- Artificial Intelligence
- Machine Tending
- Developer API
- ROS2
- Physical AI
---
