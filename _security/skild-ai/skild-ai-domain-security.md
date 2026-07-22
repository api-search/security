---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skild.ai
  spf: true
hosts:
- cert_expires: Sep 15 13:28:00 2026 GMT
  host: www.skild.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skild Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skild AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skild AI
provider_slug: skild-ai
slug: skild-ai-domain-security
source_filename: skild-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skild.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: skild.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skild-ai/refs/heads/main/security/skild-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Foundation Models
- Embodied AI
- Robot Brain
- General-Purpose Robotics
- Mobile Manipulation
- Security Robots
- Inspection Robots
- Learning From Video
- Pittsburgh
- Skild Brain
---
