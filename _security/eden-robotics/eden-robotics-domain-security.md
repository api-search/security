---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edenrobotics.ai
  spf: true
hosts:
- cert_expires: Sep  8 22:04:17 2026 GMT
  host: www.edenrobotics.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eden Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eden Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eden Robotics
provider_slug: eden-robotics
slug: eden-robotics-domain-security
source_filename: eden-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edenrobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:04:17 2026 GMT\n  hsts: false\ndomains:\n- domain: edenrobotics.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-robotics/refs/heads/main/security/eden-robotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Autonomous Robots
- Industrial Automation
- Robotics as a Service
- Artificial Intelligence
- Y Combinator
---
