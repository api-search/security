---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: robot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kiwibot.com
  spf: true
hosts:
- cert_expires: Sep 28 13:49:38 2026 GMT
  host: robot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 14:24:05 2026 GMT
  host: api.kiwibot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kiwibot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiwibot, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kiwibot
provider_slug: kiwibot
slug: kiwibot-domain-security
source_filename: kiwibot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:49:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kiwibot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 14:24:05 2026 GMT\n  hsts: null\ndomains:\n- domain: robot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kiwibot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiwibot/refs/heads/main/security/kiwibot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Autonomous Vehicles
- Delivery
- Last Mile Delivery
- Logistics
- Warehouse Automation
- Advertising
- ROS
- Open-Source
---
