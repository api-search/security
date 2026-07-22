---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ai-build.com
  spf: true
hosts:
- cert_expires: Oct  5 10:46:15 2026 GMT
  host: ai-build.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ai Build Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Build, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI Build
provider_slug: ai-build
slug: ai-build-domain-security
source_filename: ai-build-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-build.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:46:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ai-build.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-build/refs/heads/main/security/ai-build-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Artificial Intelligence
- Manufacturing
- Robotics
- CAD
- CAM
- Software
---
