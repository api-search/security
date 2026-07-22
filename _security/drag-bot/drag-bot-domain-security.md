---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dragandbot.com
  spf: true
hosts:
- cert_expires: Oct  5 08:24:55 2026 GMT
  host: www.dragandbot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drag Bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drag Bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Drag Bot
provider_slug: drag-bot
slug: drag-bot-domain-security
source_filename: drag-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dragandbot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:24:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dragandbot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drag-bot/refs/heads/main/security/drag-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Industrial Automation
- ROS
- Manufacturing
- Robot Programming
- No-Code
- Industrial Tech
- KEBA
---
