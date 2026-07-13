---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aihabitat.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: huggingface.co
  spf: true
hosts:
- cert_expires: Aug 26 20:40:33 2026 GMT
  host: aihabitat.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: huggingface.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ai Habitat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Habitat, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AI Habitat
provider_slug: ai-habitat
slug: ai-habitat-domain-security
source_filename: ai-habitat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aihabitat.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:40:33 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: huggingface.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aihabitat.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: huggingface.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/security/ai-habitat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Simulation
- Embodied AI
- Robotics
- Computer Vision
- Reinforcement Learning
- Machine Learning
- Open Source
- Research
---
