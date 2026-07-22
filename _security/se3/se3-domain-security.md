---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: se3.ai
  spf: true
hosts:
- cert_expires: Aug 22 18:29:30 2026 GMT
  host: se3.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Se3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SE3 Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SE3 Labs
provider_slug: se3
slug: se3-domain-security
source_filename: se3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: se3.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: se3.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/se3/refs/heads/main/security/se3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Spatial AI
- Autonomous Systems
- Robotics
- Computer Vision
- Defence
- Drones
---
