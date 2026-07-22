---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: remedyrobotics.com
  spf: true
hosts:
- cert_expires: Sep 21 16:41:35 2026 GMT
  host: www.remedyrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remedy Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remedy Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Remedy Robotics
provider_slug: remedy-robotics
slug: remedy-robotics-domain-security
source_filename: remedy-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.remedyrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:41:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: remedyrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remedy-robotics/refs/heads/main/security/remedy-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Robotics
- Healthcare
- Surgery
- Endovascular
- Autonomous Systems
- Cardiovascular
- Stroke
---
