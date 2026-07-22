---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sanctuary.ai
  spf: true
hosts:
- cert_expires: Oct  7 01:20:26 2026 GMT
  host: sanctuary.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sanctuary Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanctuary AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sanctuary AI
provider_slug: sanctuary-ai
slug: sanctuary-ai-domain-security
source_filename: sanctuary-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sanctuary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:20:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sanctuary.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanctuary-ai/refs/heads/main/security/sanctuary-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Humanoid Robots
- General-Purpose Robots
- Embodied AI
- Industrial Robotics
- Manufacturing
- Automotive
- Logistics
- Phoenix
- Carbon AI
- Dexterous Manipulation
- Hardware
- Vancouver
---
