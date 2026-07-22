---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aeva.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.aeva.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: resources.aeva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aeva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeva, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aeva
provider_slug: aeva
slug: aeva-domain-security
source_filename: aeva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeva.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\n- host: resources.aeva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aeva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeva/refs/heads/main/security/aeva-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- LiDAR
- 4D LiDAR
- FMCW
- Autonomous Vehicles
- Robotics
- Perception
- Sensors
- Industrial Automation
- Physical AI
---
