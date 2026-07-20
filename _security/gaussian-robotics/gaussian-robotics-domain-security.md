---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gausium.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: gs-robot.com
  spf: true
hosts:
- cert_expires: Oct 14 05:04:21 2026 GMT
  host: gausium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: developer-us.gs-robot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: openapi.gs-robot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gaussian Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gaussian Robotics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gaussian Robotics
provider_slug: gaussian-robotics
slug: gaussian-robotics-domain-security
source_filename: gaussian-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gausium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer-us.gs-robot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.gs-robot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gausium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: gs-robot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gaussian-robotics/refs/heads/main/security/gaussian-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Robotics
- Autonomous Robots
- Cleaning Robots
- IoT
- Fleet Management
- Robot Operations
---
