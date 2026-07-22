---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: telekinesis.ai
  spf: true
hosts:
- cert_expires: Aug 21 02:26:09 2026 GMT
  host: telekinesis.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telekinesisai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telekinesis.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telekinesis.ai
provider_slug: telekinesisai
slug: telekinesisai-domain-security
source_filename: telekinesisai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telekinesis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 02:26:09 2026 GMT\n  hsts: false\ndomains:\n- domain: telekinesis.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telekinesisai/refs/heads/main/security/telekinesisai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Computer Vision
- Physical AI
- Industrial Automation
- Manufacturing Automation
- 6D Pose Estimation
- Motion Planning
- Reinforcement Learning
- Python SDK
- Embodied Intelligence
- Agents
---
