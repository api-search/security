---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agibot.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.agibot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: x2-aimdk.agibot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:41:02 2026 GMT
  host: store.agibot.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agibot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgiBot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgiBot
provider_slug: agibot
slug: agibot-domain-security
source_filename: agibot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agibot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: x2-aimdk.agibot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: store.agibot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:41:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: agibot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agibot/refs/heads/main/security/agibot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Humanoid Robots
- Embodied AI
- Artificial Intelligence
- Manufacturing
- Hardware
- Middleware
- ROS 2
- gRPC
- Protocol Buffers
- Simulation
- Machine Learning
- Open Source
- Model Context Protocol
- Agentic Commerce
- China
---
