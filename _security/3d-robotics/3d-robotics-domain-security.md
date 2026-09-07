---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3dr.com
  spf: true
hosts:
- cert_expires: Nov  7 16:59:20 2026 GMT
  host: www.3dr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3D Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3DR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3DR
provider_slug: 3d-robotics
slug: 3d-robotics-domain-security
source_filename: 3d-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3dr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 16:59:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 3dr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3d-robotics/refs/heads/main/security/3d-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Drones
- UAV
- Robotics
- Hardware
- Autopilots
- GNSS
- Telemetry
- Electronics Manufacturing
- Open Source Hardware
---
