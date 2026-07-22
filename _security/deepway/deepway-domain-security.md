---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deepway.com
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: deepway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepWay 深向, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DeepWay 深向
provider_slug: deepway
slug: deepway-domain-security
source_filename: deepway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: deepway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepway/refs/heads/main/security/deepway-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Automotive
- Autonomous Vehicles
- Electric Vehicles
- Trucking
- Logistics
- Fleet Management
- Autonomous Driving
- New Energy
- Robotics
- China
---
