---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tera-ai.com
  spf: false
hosts:
- cert_expires: Oct  1 12:38:34 2026 GMT
  host: tera-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tera Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tera-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tera-ai
provider_slug: tera-ai
slug: tera-ai-domain-security
source_filename: tera-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tera-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:38:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tera-ai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tera-ai/refs/heads/main/security/tera-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Artificial Intelligence
- Autonomous Navigation
- Spatial AI
- Computer Vision
- Foundation Models
- Autonomy
---
