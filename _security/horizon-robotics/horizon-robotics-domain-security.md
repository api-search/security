---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: horizon.auto
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: www.horizon.auto
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: mcp.oe.horizon.auto
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Horizon Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horizon Robotics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Horizon Robotics
provider_slug: horizon-robotics
slug: horizon-robotics-domain-security
source_filename: horizon-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.horizon.auto\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.oe.horizon.auto\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: horizon.auto\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-robotics/refs/heads/main/security/horizon-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automotive
- Autonomous Driving
- Semiconductors
- Robotics
- Edge AI
- Machine Learning
- Model Context Protocol
- Agent Skills
- Developer Tools
- China
---
