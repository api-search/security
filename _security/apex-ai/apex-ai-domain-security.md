---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apex.ai
  spf: true
hosts:
- cert_expires: Oct 12 04:30:40 2026 GMT
  host: www.apex.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apex Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apex.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apex.AI
provider_slug: apex-ai
slug: apex-ai-domain-security
source_filename: apex-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:30:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: apex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apex-ai/refs/heads/main/security/apex-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Embedded
- Autonomous Vehicles
- Robotics
- Middleware
- Software Defined Vehicle
- ROS 2
- Automotive
- Safety Critical
---
