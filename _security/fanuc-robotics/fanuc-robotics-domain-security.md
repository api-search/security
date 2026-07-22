---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fanuc.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.fanuc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fanuc Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FANUC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FANUC
provider_slug: fanuc-robotics
slug: fanuc-robotics-domain-security
source_filename: fanuc-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fanuc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fanuc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fanuc-robotics/refs/heads/main/security/fanuc-robotics-domain-security.yml
summary_line: TLSv1.3
tags:
- Industrial Robotics
- CNC
- Factory Automation
- Collaborative Robots
- Machine Tools
- Injection Molding
- Wire EDM
- Manufacturing
- Industrial IoT
- FOCAS
- KAREL
- ROS 2
- MTConnect
- OPC UA
- Hardware
---
