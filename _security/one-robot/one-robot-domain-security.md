---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: onerobot.io
  spf: false
hosts:
- cert_expires: Aug 22 05:02:31 2026 GMT
  host: www.onerobot.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Robot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Robot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: One Robot
provider_slug: one-robot
slug: one-robot-domain-security
source_filename: one-robot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onerobot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:02:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: onerobot.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-robot/refs/heads/main/security/one-robot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Simulation
- Artificial Intelligence
- Machine Learning
- World Models
- Y Combinator
---
