---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: peerrobotics.ai
  spf: true
hosts:
- cert_expires: Sep 30 11:14:10 2026 GMT
  host: peerrobotics.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peer Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peer Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Peer Robotics
provider_slug: peer-robotics
slug: peer-robotics-domain-security
source_filename: peer-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peerrobotics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:14:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peerrobotics.ai\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peer-robotics/refs/heads/main/security/peer-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Autonomous Mobile Robots
- Manufacturing
- Warehouse Automation
- Material Handling
- Hardware
---
