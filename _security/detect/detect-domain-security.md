---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: detecttechnologies.com
  spf: true
hosts:
- cert_expires: Oct 14 23:33:30 2026 GMT
  host: detecttechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Detect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Detect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Detect
provider_slug: detect
slug: detect-domain-security
source_filename: detect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: detecttechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: detecttechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/detect/refs/heads/main/security/detect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Saas
- Industrial AI
- IoT
- Computer Vision
- Workplace Safety
- Predictive Maintenance
- Drones
- Robotics
---
