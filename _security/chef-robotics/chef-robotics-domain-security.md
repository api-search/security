---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chefrobotics.ai
  spf: true
hosts:
- cert_expires: Sep 12 13:55:22 2026 GMT
  host: www.chefrobotics.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chef Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chef Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chef Robotics
provider_slug: chef-robotics
slug: chef-robotics-domain-security
source_filename: chef-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chefrobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:55:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chefrobotics.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chef-robotics/refs/heads/main/security/chef-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Food Robotics
- Food Manufacturing
- Meal Assembly
- Physical AI
- Embodied AI
- Vision Language Action
- Foundation Models
- ChefOS
- Robotics As A Service
- Manipulation
- Manufacturing Automation
- Hardware
---
