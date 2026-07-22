---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: veobot.com
  spf: true
hosts:
- cert_expires: Sep 19 21:06:30 2026 GMT
  host: veobot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veo Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veo Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Veo Robotics
provider_slug: veo-robotics
slug: veo-robotics-domain-security
source_filename: veo-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:06:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veobot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veo-robotics/refs/heads/main/security/veo-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Robotics
- Industrial Automation
- Machine Safety
- Computer Vision
- Manufacturing
---
